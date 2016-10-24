---
title: PreApprovedAddons
description: PreApprovedAddons
MSHAttr:
- 'PreferredSiteName:MSDN'
- 'PreferredLib:/library/windows/hardware'
ms.assetid: 95143c24-f5be-45e5-8028-4b254692797b
ms.prod: W10
ms.mktglfcycl: deploy
ms.sitesec: msdn
---

# PreApprovedAddons


**Important**  
This setting has been deprecated in Windows® 8.1. The information about this deprecated setting is provided for reference only. Add-ons can still be installed but they will be disabled, by default. Users will be able to choose the add-ons to enable.

 

`PreapprovedAddons` contains settings for configuring Internet Explorer® pre-approved add-ons.

Pre-approved add-ons are plug-in modules used to add functionality to Internet Explorer.

`PreapprovedAddons` can contain one or more [AddonGuidItem](microsoft-windows-ie-internetexplorerpreapprovedaddonsaddonguiditem.md) settings each of which represents a single add-on module.

## Child Elements


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p>[AddonGuidItem](microsoft-windows-ie-internetexplorerpreapprovedaddonsaddonguiditem.md)</p></td>
<td><p>Specifies settings for an add-on module.</p></td>
</tr>
</tbody>
</table>

 

## Valid Passes


specialize

## Parent Hierarchy


[Microsoft-Windows-IE-InternetExplorer](microsoft-windows-ie-internetexplorer-win7-microsoft-windows-ie-internetexplorer.md) | **PreapprovedAddons**

## Applies To


For a list of the supported Windows® editions and architectures that this component supports, see [Microsoft-Windows-IE-InternetExplorer](microsoft-windows-ie-internetexplorer-win7-microsoft-windows-ie-internetexplorer.md).

## XML Example


The following XML output shows how to set two Internet Explorer pre-approved add-ons.

``` syntax
<PreapprovedAddons>
  <AddonGuidItem>
    <AddonGuid>{a1b1c123d1e1f4a5a6a7aa8a9a0a}</AddonGuid>
  </AddonGuidItem>
  <AddonGuidItem>
    <AddonGuid>{b1c123d1e1f4a5a6a7aa8a9a0a33}</AddonGuid>
  </AddonGuidItem>
</PreapprovedAddons>
```

## Related topics


[Microsoft-Windows-IE-InternetExplorer](microsoft-windows-ie-internetexplorer-win7-microsoft-windows-ie-internetexplorer.md)

[InstalledBHOList](microsoft-windows-ie-internetexplorerinstalledbholist.md)

[InstalledBrowserExtensions](microsoft-windows-ie-internetexplorerinstalledbrowserextensions.md)

[InstalledToolbarsList](microsoft-windows-ie-internetexplorerinstalledtoolbarslist.md)

 

 

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20%5Bp_unattend\p_unattend%5D:%20PreApprovedAddons%20%20RELEASE:%20%2810/3/2016%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/default.aspx. "Send comments about this topic to Microsoft")





