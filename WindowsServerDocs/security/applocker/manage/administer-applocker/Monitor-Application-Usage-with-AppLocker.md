---
title: Monitor Application Usage with applocker
ms.custom: na
ms.prod: windows-server-2012
ms.reviewer: na
ms.suite: na
ms.technology: 
  - techgroup-security
ms.tgt_pltfrm: na
ms.topic: article
ms.assetid: 70f8b150-2948-4554-94e1-c611a1ba2907
---
# Monitor Application Usage with applocker
This topic describes how to monitor application usage when applocker policies are applied in Windows Server® 2012 and Windows® 8.

Once you set rules and deploy the applocker policies, it is good practice to determine if the policy implementation is what you expected.

### <a name="BKMK_AppLkr_Disc_Effect_Pol"></a>Discover the effect of an applocker policy
You can evaluate how the applocker policy is currently implemented for documentation or audit purposes, or before you modify the policy. Updating your applocker Policy Deployment Planning document will help you track your findings. For information about creating this document, see [Creating Your applocker Planning Document](http://technet.microsoft.com/library/ee449479(WS.10).aspx). You can perform one or more of the following steps to understand what application controls are currently enforced through applocker rules.

-   **Analyze the applocker logs in Event Viewer**

    When applocker policy enforcement is set to **Enforce rules**, rules are enforced for the rule collection and all events are audited. When applocker policy enforcement is set to **Audit only**, rules are not enforced but are still evaluated to generate audit event data that is written to the applocker logs.

    For the procedure to access the log, see [View the applocker Log in Event Viewer](#BKMK_AppLkr_View_Log).

-   **Enable the Audit only applocker enforcement setting**

    By using the **Audit only** enforcement setting, you can ensure that the applocker rules are properly configured for your organization. When applocker policy enforcement is set to **Audit only**, rules are only evaluated but all events generated from that evaluation are written to the applocker log.

    For the procedure to do this, see [Configure an applocker Policy for Audit Only]().

-   **Review applocker events with Get\-applockerFileInformation**

    For both event subscriptions and local events, you can use the **Get\-applockerFileInformation** Windows PowerShell cmdlet to determine which files have been blocked or would have been blocked \(if you are using the audit\-only enforcement mode\) and how many times the event has occurred for each file.

    For the procedure to do this, see [Review applocker Events with Get\-applockerFileInformation](#BKMK_AppLkr_Review_Events).

-   **Review applocker events with Test\-applockerPolicy**

    You  can use the **Test\-applockerPolicy** Windows PowerShell cmdlet to determine determine whether any of the rules in your rule collections will be blocked on your reference computer or the computer on which you maintain policies.

    For the procedure to do this, see [Test an applocker Policy by Using Test-applockerPolicy]().

### <a name="BKMK_AppLkr_Review_Events"></a>Review applocker events with Get\-applockerFileInformation
For both event subscriptions and local events, you can use the **Get\-applockerFileInformation** Windows PowerShell cmdlet to determine which files have been blocked or would have been blocked \(if the **Audit only** enforcement setting is applied\) and how many times the event has occurred for each file.

Membership in the local **Administrators** group, or equivalent, is the minimum required to complete this procedure.

> [!NOTE]
> If the applocker logs are not on the local computer, you will need permission to view the logs. If the output is saved to a file, you will need permission to read that file.

##### To review applocker events with Get\-applockerFileInformation

1.  Open a Command Prompt window.

2.  At the command prompt, type **PowerShell**, and then press ENTER.

3.  Run the following command to review how many times a file would have been blocked from running if rules were enforced:

    `Get-applockerFileInformation –EventLog –Logname "Microsoft-Windows-applocker\EXE and DLL" –EventType Audited –Statistics`

    > [!NOTE]
    > For an event subscription, specify the path to the forwarded event log for the Logname parameter.

4.  Run the following command to review how many times a file has been allowed to run or prevented from running:

    `Get-applockerFileInformation –EventLog –Logname "Microsoft-Windows-applocker\EXE and DLL" –EventType Allowed –Statistics`

### <a name="BKMK_AppLkr_View_Log"></a>View the applocker Log in Event Viewer
When applocker policy enforcement is set to **Enforce rules**, rules are enforced for the rule collection and all events are audited. When applocker policy enforcement is set to **Audit only**, rules are only evaluated but all events generated from that evaluation are written to the applocker log.

Membership in the local **Administrators** group, or equivalent, is the minimum required to complete this procedure.

##### To view events in the applocker log by using Event Viewer

1.  Open Event Viewer. To do this, click **Start**, type **eventvwr.msc** in the **Search programs and files** box, and then press ENTER.

2.  In the console tree under **Application and Services Logs\\Microsoft\\Windows**, double\-click **applocker**.

applocker events are listed in either the **EXE and DLL** log, the **MSI and Script** log, or the **Packaged app\-Deployment** or **Packaged app\-Execution** log. Event information includes the enforcement setting, file name, date and time, and user name. The logs can be exported to other file formats for further analysis.

## See Also
[applocker Overview \[Client\]](assetId:///1637ae87-5059-4d95-8c68-96f35cbc88c7)

