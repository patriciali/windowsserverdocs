---
title: bitsadmin getfilestransferred
ms.custom: na
ms.prod: windows-server-2012
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.assetid: e282815c-938b-4ac0-a09d-9baafb656dcb
---
# bitsadmin getfilestransferred
Retrieves the number of files transferred for the specified job.

## Syntax

```
bitsadmin /GetFilesTransferred <Job>
```

## Parameters

|Parameter|Description|
|-------------|---------------|
|Job|The job's display name or GUID|

## <a name="BKMK_examples"></a>Examples
The following example retrieves the number of files transferred in the job named *myDownloadJob*.

```
C:\>bitsadmin /GetFilesTransferred myDownloadJob
```

## additional references
[Command-Line Syntax Key](../commandline-syntax-key.md)

