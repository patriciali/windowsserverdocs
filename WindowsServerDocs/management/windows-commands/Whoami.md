---
title: whoami
ms.custom: na
ms.prod: windows-server-2012
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.assetid: 6e3f4d5c-f1f5-4429-b602-afad2b3488bf
---
# whoami
Displays user, group and privileges information for the user who is currently logged on to the local system. if used without parameters, **whoami** displays the current domain and user name.

for examples of how to use this command, see [Examples](#BKMK_examples).

## Syntax

```
whoami [/upn | /fqdn | /logonid]
whoami {[/user] [/groups] [/priv]} [/fo <format>] [/nh]
whoami /all [/fo <format>] [/nh]
```

## Parameters

|Parameter|Description|
|-------------|---------------|
|\/upn|Displays the user name in user principal name \(UPN\) format.|
|\/fqdn|Displays the user name in fully qualified domain name \(FQDN\) format.|
|\/logonid|Displays the logon ID of the current user.|
|\/user|Displays the current domain and user name and the security identifier \(SID\).|
|\/groups|Displays the user groups to which the current user belongs.|
|\/priv|Displays the security privileges of the current user.|
|\/fo <format>|Specifies the output format. Valid values include:<br /><br />**table** Displays output in a table. This is the default value.<br /><br />**list** Displays output in a list.<br /><br />**csv** Displays output in comma\-separated value \(CSV\) format.|
|\/all|Displays all information in the current access token, including the current user name, security identifiers \(SID\), privileges, and groups that the current user belongs to.|
|\/nh|Specifies that the column header should not be displayed in the output. This is valid only for table and CSV formats.|
|\/?|Displays help at the command prompt.|

## <a name="BKMK_examples"></a>Examples
To display the domain and user name of the person who is currently logged on to this computer, type:

```
whoami
```

Output similar to the following appears:

```
DOMAIN1\administrator
```

To display all of the information in the current access token, type:

```
whoami /all
```

#### additional references
[Command-Line Syntax Key](commandline-syntax-key.md)

