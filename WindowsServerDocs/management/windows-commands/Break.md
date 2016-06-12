---
title: break
ms.custom: na
ms.prod: windows-server-2012
ms.reviewer: na
ms.suite: na
ms.technology: 
  - techgroup-storage
ms.tgt_pltfrm: na
ms.topic: article
ms.assetid: ffc4901c-457b-46a6-a671-3052355f8a3c
---
# break
breaks the mirrored volume with focus into two simple volumes.

for examples of how this command can be used, see [Examples](#BKMK_examples).

## Syntax

```
break disk=<n> [nokeep] [noerr]
```

## Parameters

|Parameter|Description|
|-------------|---------------|
|disk\=<n>|Specifies the disk that contains the mirrored volume. This disk is given focus and does not retain the drive letter or any mount points. if the specified disk is the current system or startup disk, the command fails.|
|nokeep|Specifies that only one of the mirrored volumes is retained; the simple volume on disk N is deleted and converted to free space. Neither the volume nor the free space receives the focus.|
|noerr|for scripting only. When an error is encountered, DiskPart continues to process commands as if the error did not occur. Without this parameter, an error causes DiskPart to exit with an error code.|

## remarks

-   Applies to dynamic disks only. breaks the mirrored volume with focus into two simple volumes. One simple volume retains the drive letter and any mount points of the mirrored volume. The other simple volume receives the focus so you can assign it a drive letter.

-   By default, the contents of both halves of the mirror are retained. Each half becomes a simple volume. By using the nokeep parameter, you retain only one half of the mirror as a simple volume, and the other half is deleted and converted to free space. Neither volume receives the focus.

-   A mirrored volume must be selected for this operation to succeed. Use the **select volume** command to select a mirrored volume and shift the focus to it.

## <a name="BKMK_examples"></a>Examples
To break the mirrored disk 2 into two simple volumes, type:

```
break disk=2
```

#### additional references
[Command-Line Syntax Key](commandline-syntax-key.md)

[Diskpart \[LH\]](assetId:///26a4a166-95fa-4faf-95bc-2d5345f4a57a)

