---
title: PageFile
description: PageFile
MSHAttr:
- 'PreferredSiteName:MSDN'
- 'PreferredLib:/library/windows/hardware'
ms.assetid: a9d773c1-dd21-4b38-83a0-ecd65c9b1529
ms.prod: W10
ms.mktglfcycl: deploy
ms.sitesec: msdn
---

# PageFile


`PageFile` specifies the location and the size of the Windows PE operating system page file to create. This setting applies only to the Windows PE page file, and not to the page file of the Windows installation.

## Child Elements


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p>[Path](path-win7-microsoft-windows-setuppagefilepath.md)</p></td>
<td><p>Specifies the path of the page file to create.</p></td>
</tr>
<tr class="even">
<td><p>[Size](size-win7-microsoft-windows-setuppagefilesize.md)</p></td>
<td><p>Specifies the size of the page file to create.</p></td>
</tr>
</tbody>
</table>

 

## Valid Passes


windowsPE

## Parent Hierarchy


[Microsoft-Windows-Setup](microsoft-windows-setup-win7-microsoft-windows-setup.md) | **PageFile**

## Applies To


For the list of the supported Windows editions and architectures that this component supports, see [Microsoft-Windows-Setup](microsoft-windows-setup-win7-microsoft-windows-setup.md).

## XML Example


The following XML output shows how to create a page file.

``` syntax
<PageFile>
   <Path>%WINDIR%\MyPagefile.sys</Path>
   <Size>512</Size>
</PageFile>
```

## Related topics


[Microsoft-Windows-Setup](microsoft-windows-setup-win7-microsoft-windows-setup.md)

 

 

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20%5Bp_unattend\p_unattend%5D:%20PageFile%20%20RELEASE:%20%2810/3/2016%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/default.aspx. "Send comments about this topic to Microsoft")





