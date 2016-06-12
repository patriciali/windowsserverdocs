---
title: select volume
ms.custom: na
ms.prod: windows-server-2012
ms.reviewer: na
ms.suite: na
ms.technology: 
  - techgroup-storage
ms.tgt_pltfrm: na
ms.topic: article
ms.assetid: 5d70d776-80ad-4f20-8288-a7997fb1df28
---
# select volume
selects the specified volume and shifts the focus to it. This command can also be used to display the volume that currently has the focus in the selected disk.

for examples of how this command can be used, see [Examples](#BKMK_examples).

## Syntax

```
select volume={<n>|<d>}
```

## Parameters

|Parameter|Description|
|-------------|---------------|
|<n>|The number of the volume to receive the focus. You can view the numbers for all volumes on the disk currently selected by using the **list volume** command in DiskPart.|
|<d>|The drive letter or mount point path of the volume to receive the focus.|

## remarks

-   if no volume is specified, this command displays the volume that currently has the focus in the selected disk.

-   On a basic disk, selecting a volume also gives the focus to the corresponding partition.

-   if a volume is selected with a corresponding partition, the partition will be automatically selected.

-   if a partition is selected with a corresponding volume, the volume will be automatically selected.

## <a name="BKMK_examples"></a>Examples
To shift the focus to volume 2, type:

```
select volume=2
```

To shift the focus to drive C, type:

```
select volume=c
```

To shift the focus to the volume mounted on a folder named "mountpath", type:

```
select volume=c:\mountpath
```

To display the volume that currently has the focus in the selected disk, type:

```
select volume
```

#### additional references
[Command-Line Syntax Key](../commandline-syntax-key.md)

[Diskpart \[LH\]](assetId:///26a4a166-95fa-4faf-95bc-2d5345f4a57a)

