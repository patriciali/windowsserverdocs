---
title: Export an applocker Policy from a GPO
ms.custom: na
ms.prod: windows-server-2012
ms.reviewer: na
ms.suite: na
ms.technology: 
  - techgroup-security
ms.tgt_pltfrm: na
ms.topic: article
ms.assetid: 030198d3-5964-4f7e-b61e-8b2f241bb375
---
# Export an applocker Policy from a GPO
This topic describes the steps to export an applocker policy from a Group Policy Object \(GPO\) so that it can be modified in  Windows Server 2012  and Windows 8.

Updating an applocker policy that is currently enforced in your production environment can have unintended results. Therefore, export the policy from the GPO and update the rule or rules by using applocker on your applocker reference or test computer.

To complete this procedure, you must have Edit Setting permission to edit a GPO. By default, members of the **Domain Admins** group, the **Enterprise Admins** group, and the **Group Policy Creator Owners** group have this permission.

#### Export the policy from the GPO

1.  In the Group Policy Management Console \(GPMC\), open the GPO that you want to edit.

2.  In the console tree under **Computer Configuration\\Policies\\Windows Settings\\Security Settings\\Application Control Policies**, click **applocker**.

3.  Right\-click **applocker**, and then click **Export Policy**.

4.  In the **Export Policy** dialog box, type a name for the exported policy \(for example, the name of the GPO\), select a location to save the policy, and then click **Save**.

5.  The **applocker** dialog box will notify you of how many rules were exported. Click **OK**.

