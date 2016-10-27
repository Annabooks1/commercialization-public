---
title: Size
description: Size
MSHAttr:
- 'PreferredSiteName:MSDN'
- 'PreferredLib:/library/windows/hardware'
ms.assetid: 290c7bde-7570-4d3b-a724-36b6a0779c24
ms.prod: W10
ms.mktglfcycl: deploy
ms.sitesec: msdn
---

# Size


`Size` specifies the size, in megabytes, of the page file to create for [PageFile](microsoft-windows-setuppagefile.md).

## Values


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><em>size_of_the_page_file_in_megabytes</em></p></td>
<td><p>Specifies the size of the page file to create, in megabytes.</p>
<p>If this value is set, but there is no path specified to a page file, this value is applied to the default page file on the computer.</p></td>
</tr>
</tbody>
</table>

 

## Valid Passes


windowsPE

## Parent Hierarchy


[Microsoft-Windows-Setup](microsoft-windows-setup.md) | [PageFile](microsoft-windows-setuppagefile.md) | **Size**

## Applies To


For the list of the supported Windows editions and architectures that this component supports, see [Microsoft-Windows-Setup](microsoft-windows-setup.md).

## XML Example


The following XML output shows how to create a page file.

``` syntax
<PageFile>
   <Path>%WINDIR%\MyPagefile.sys</Path>
   <Size>512</Size>
</PageFile>
```

## Related topics


[PageFile](microsoft-windows-setuppagefile.md)

 

 

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20%5Bp_unattend\p_unattend%5D:%20Size%20%20RELEASE:%20%2810/3/2016%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/default.aspx. "Send comments about this topic to Microsoft")





