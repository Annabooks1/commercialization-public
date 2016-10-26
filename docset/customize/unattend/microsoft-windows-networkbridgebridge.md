---
title: Bridge
description: Bridge
MSHAttr:
- 'PreferredSiteName:MSDN'
- 'PreferredLib:/library/windows/hardware'
ms.assetid: 2edee894-f32f-45db-b058-449cddca9cdd
ms.prod: W10
ms.mktglfcycl: deploy
ms.sitesec: msdn
---

# Bridge


`Bridge` specifies the adapters to bridge together to form a home network. This entry requires at least two adapters.

**Note**  
Not all adapters can be bridged.

 

## Values


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><em>Bridge</em></p></td>
<td><p>Specifies the adapters. <em>Bridge</em> is a comma-delimited list.</p></td>
</tr>
</tbody>
</table>

 

This string type does not support empty elements. Do not create an empty value for this setting.

## Valid Passes


generalize

## Parent Hierarchy


[Microsoft-Windows-NetworkBridge](microsoft-windows-networkbridge.md) | **Bridge**

## Applies To


For a list of the supported Windows® editions and architectures that this component supports, see [Microsoft-Windows-NetworkBridge](microsoft-windows-networkbridge-win7-microsoft-windows-networkbridge.md).

## XML Example


The following XML output shows how to set the bridge.

``` syntax
<Bridge>{A123B456-C789-DE00-FFA4-E73F7B925305},{123F654D-00FF-AABB-CCDD1-EEFF7777702}</Bridge>
```

## Related topics


[Microsoft-Windows-NetworkBridge](microsoft-windows-networkbridge-win7-microsoft-windows-networkbridge.md)

[Microsoft-Windows-SharedAccess](microsoft-windows-sharedaccess-win7-microsoft-windows-sharedaccess.md)

 

 

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20%5Bp_unattend\p_unattend%5D:%20Bridge%20%20RELEASE:%20%2810/3/2016%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/default.aspx. "Send comments about this topic to Microsoft")





