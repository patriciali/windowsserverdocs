---
title: expand
ms.custom: na
ms.prod: windows-server-2012
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.assetid: 66de0488-a0c4-40c2-9b03-e40c107ba343
author: jaimeo
---
# expand
expands one or more compressed files. You can use this command to retrieve compressed files from distribution disks.  
  
## Syntax  
  
```  
expand [/r] <source> <destination>  
  
expand /r <source> [<destination>]  
  
expand /i <source> [<destination>]  
  
expand /d <source>.cab [/f:<files>]  
  
expand <source>.cab /f:<files> <destination>  
```  
  
### Parameters  
  
|Parameter|Description|  
|-------------|---------------|  
|\/r|renames expanded files.|  
|source|Specifies the files to expand. *Source* can consist of a drive letter and colon, a directory name, a file name, or a combination of these. You can use wildcards \(**\*** or **?**\).|  
|destination|Specifies where files are to be expanded.<br /><br />if *source* consists of multiple files and you do not specify **\/r**, *destination* must be a directory.<br /><br />*Destination* can consist of a drive letter and colon, a directory name, a file name, or a combination of these.<br /><br />Destination file &#124; path specification.|  
|\/i|renames expanded files but ignores the directory structure.<br /><br />This parameter applies to:  Windows Server 2008 R2  and  Windows 7 .|  
|\/d|Displays a list of files in the source location. Does not expand or extract the files.|  
|\/f:|Specifies the files in a cabinet \(.cab\) file that you want to expand. You can use wildcards \(**\*** or **?**\).|  
|\/?|Displays help at the command prompt.|  
  
## remarks  
  
-   Using **expand** at the recovery Console  
  
    The **expand** command, with different parameters, is available from the recovery Console. for more information about the recovery Console, see [article 314058](http://support.microsoft.com/kb/314058) in the Microsoft Knowledge Base.  
  
## additional references  
[Command-Line Syntax Key](commandline-syntax-key.md)  
  
[Command-Line Reference_1](Command-Line-Reference_1.md)  
  
