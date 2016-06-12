---
title: manage-bde: changekey
ms.custom: na
ms.prod: windows-server-2012
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.assetid: 69463db9-7e03-47ff-b233-a95d5055725f
---
# manage-bde: changekey
Modifies the startup key for an operating system drive. for examples of how this command can be used, see [Examples](#BKMK_Examples).

## Syntax

```
manage-bde -changekey [<Drive>] [<pathToExternalKeydirectory>] [-computername <Name>] [{-?|/?}] [{-help|-h}]
```

### Parameters

|Parameter|Description|
|-------------|---------------|
|<Drive>|Represents a drive letter followed by a colon.|
|<pathToExternalKeydirectory>|Represents the directory location to save the external startup key file that can be used to unlock the drive.|
|\-computername|Specifies that manage\-bde.exe will be used to modify BitLocker protection on a different computer. You can also use **\-cn** as an abbreviated version of this command.|
|<Name>|Represents the name of the computer on which to modify BitLocker protection. Accepted values include the computer's NetBIOS name and the computer's IP address.|
|\-? or \/?|Displays brief help at the command prompt.|
|\-help or \-h|Displays complete help at the command prompt.|

## <a name="BKMK_Examples"></a>Examples
The following example illustrates using the **\-changekey** command to create a new startup key on drive E to use with BitLocker encryption on drive C.

```
manage-bde –changekey C: E:\
```

## additional references

-   [Command-Line Syntax Key](../commandline-syntax-key.md)

-   [manage-bde]()

