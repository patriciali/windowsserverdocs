---
title: Create Your applocker Rules
ms.custom: na
ms.prod: windows-server-2012-r2
ms.reviewer: na
ms.suite: na
ms.technology: 
  - techgroup-security
ms.tgt_pltfrm: na
ms.topic: article
ms.assetid: 72cd1356-1e25-499b-93d9-1e3e5b204cbc
---
# Create Your applocker Rules
This topic for the IT professional describes what you need to know about applocker rules and the methods that you can to create rules.

## Creating applocker rules
applocker rules apply to the targeted application, and they are the components that make up the applocker policy. Depending on your IT environment and the business group that requires application control policies, setting these access rules for each application can be time\-consuming and prone to error. With applocker, you can generate rules automatically or create rules individually. Creating rules that are derived from your planning document can help you avoid unintended results. For information about this planning document and other planning activities, see [applocker Policies Design Guide]().

### Automatically generate your rules
You can use a reference computer to automatically create a set of default rules for each of the installed applications, test and modify each rule as necessary, and deploy the policies. Creating most of the rules for all the installed applications gives you a starting point to build and test your policies. For information about performing this task, see the following topics:

-   [Configure the applocker Reference Computer](assetId:///615506e9-fc32-4003-a241-01794c3a9bd3)

-   [Run the Automatically Generate Rules Wizard]()

-   [Create applocker Default Rules]()

-   [Edit applocker Rules]()

-   [Configure Exceptions for an applocker Rule]()

### Create your rules individually
You can create rules and set the mode to **Audit only** for each installed application, test and update each rule as necessary, and then deploy the policies. Creating rules individually might be best when you are targeting a small number of applications within a business group.

> [!NOTE]
> applocker includes default rules for each rule collection. These rules are intended to help ensure that the files that are required for Windows to operate properly are allowed in an applocker rule collection. You can also edit the default rules. For information about creating the default rules for the Windows operating system, see [Create applocker Default Rules]().

For information about performing this task, see:

1.  [Create a Rule That Uses a Publisher Condition]()

2.  [Create a Rule That Uses a Path Condition]()

3.  [Create a Rule That Uses a File Hash Condition]()

4.  [Edit applocker Rules]()

5.  [Enforce applocker Rules]()

6.  [Configure an applocker Policy for Audit Only]()

## About selecting rules
applocker policies are composed of distinct rules for specific applications. These rules are grouped by collection, and they are implemented through an applocker policy definition. applocker policies are managed by using Group Policy or by using the Local Security Policy snap\-in for a single computer.

When you determine what types of rules to create for each of your business groups or organizational units \(OUs\), you should also determine what enforcement setting to use for each group. Certain rule types are more applicable for some applications, depending on how the applications are deployed in a specific business group.

For information about how to determine and document your applocker rules, see [applocker Policies Design Guide]().

For information about applocker rules and applocker policies, see the following topics:

-   [Understanding applocker Rule Behavior]()

-   [Understanding applocker Rule Exceptions]()

-   [Understanding applocker Rule Collections]()

-   [Understanding applocker Allow and Deny Actions on Rules]()

-   [Understanding applocker Rule Condition Types]()

-   [Understanding applocker Default Rules]()

## Next steps

1.  [Import an applocker Policy into a GPO]()

2.  [Import an applocker Policy from Another Computer]()

3.  [Test and Update an applocker Policy]()

4.  [Deploy the applocker Policy into Production]()

## See Also
[Create Your applocker Policies]()

