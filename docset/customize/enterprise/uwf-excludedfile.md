---
title: UWF\_ExcludedFile
description: UWF\_ExcludedFile
MSHAttr:
- 'PreferredSiteName:MSDN'
- 'PreferredLib:/library/windows/hardware'
ms.assetid: a63710d5-2135-4a52-a891-ea2c370ca593
ms.author: windows-hardware-design-content
ms.date: 05/02/2017
ms.topic: article
ms.prod: windows-hardware
ms.technology: windows-devices
---

# UWF\_ExcludedFile


Contains the files and folders that are currently in the file exclusion list for a volume protected by Unified Write Filter (UWF).

## Syntax


``` syntax
class UWF_ExcludedFile {
    [Read] string FileName;
};
```

## Members


The following tables list any methods and properties that belong to this class.

### <a href="" id="pro"></a>Properties

<table>
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th>Property</th>
<th>Data type</th>
<th>Qualifier</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p>FileName</p></td>
<td><p>string</p></td>
<td><p>[read]</p></td>
<td><p>The name of the file or folder path in the file exclusion list, including the full path relative to the volume.</p></td>
</tr>
</tbody>
</table>

 

### Remarks

UWF\_ExcludedFile does not represent an actual WMI object, and you cannot use this class to get or set file exclusions.

You must use the [UWF\_Volume.GetExclusions](uwf-volumegetexclusions.md) method to retrieve UWF\_ExcludedFile objects.

You can use the [UWF\_Volume.AddExclusion](uwf-volumeaddexclusion.md) and [UWF\_Volume.RemoveExclusion](uwf-volumeremoveexclusion.md) methods to add or remove file and folder exclusions to a volume.

## Requirements


|                       |           |
|-----------------------|-----------|
| Windows Edition       | Supported |
| Windows 10 Home       | No        |
| Windows 10 Pro        | No        |
| Windows 10 Enterprise | Yes       |
| Windows 10 Education  | Yes       |

 

## Related topics


[Unified Write Filter WMI provider reference](uwf-wmi-provider-reference.md)

[Unified Write Filter](unified-write-filter.md)

 

 

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20%5Bp_enterprise_customizations\p_enterprise_customizations%5D:%20UWF_ExcludedFile%20%20RELEASE:%20%2810/17/2016%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/en-us/default.aspx. "Send comments about this topic to Microsoft")





