---
title: convert mbr
ms.custom: na
ms.prod: windows-server-2012
ms.reviewer: na
ms.suite: na
ms.technology: 
  - techgroup-storage
ms.tgt_pltfrm: na
ms.topic: article
ms.assetid: a635a4c0-af73-4330-b021-51d483424537
---
# convert mbr
converts an empty basic disk with the GUID Partition Table \(gpt\) partition style into a basic disk with the master boot record \(MBR\) partition style.

> [!importANT]
> The disk must be empty to convert it into an MBR disk. Back up your data, and then delete all partitions or volumes before converting the disk.

for instructions regarding how to use this command, see [change a GUID Partition Table Disk into a Master Boot Record Disk](http://go.microsoft.com/fwlink/?LinkId=207050) \(http:\/\/go.microsoft.com\/fwlink\/?LinkId\=207050\).

## Syntax

```
convert mbr [noerr]
```

## Parameters

|Parameter|Description|
|-------------|---------------|
|noerr|for scripting only. When an error is encountered, DiskPart continues to process commands as if the error did not occur. Without this parameter, an error causes DiskPart to exit with an error code.|

## remarks

-   A basic disk must be selected for this operation to succeed. Use the **select disk** command to select a basic disk and shift the focus to it.

## <a name="BKMK_examples"></a>Examples
To convert a basic disc from gpt partition style to MBR partition style, type>:

```
convert mbr
```

#### additional references
[Command-Line Syntax Key](../commandline-syntax-key.md)

[Diskpart \[LH\]](assetId:///26a4a166-95fa-4faf-95bc-2d5345f4a57a)

