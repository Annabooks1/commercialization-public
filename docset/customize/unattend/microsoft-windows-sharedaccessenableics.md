---
title: EnableICS
description: EnableICS
MSHAttr:
- 'PreferredSiteName:MSDN'
- 'PreferredLib:/library/windows/hardware'
ms.assetid: 3e26f9dd-a079-4b0a-aece-a1501dd54c35
ms.prod: W10
ms.mktglfcycl: deploy
ms.sitesec: msdn
---

# EnableICS


`EnableICS` specifies whether Internet-connection sharing is enabled.

This setting has no effect on Server Core installations of Windows Server® 2008, Windows Server 2008 R2, and Windows Server 2012.

## Values


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><strong>true</strong></p></td>
<td><p>Enables Internet-connection sharing.</p></td>
</tr>
<tr class="even">
<td><p><strong>false</strong></p></td>
<td><p>Disables Internet-connection sharing. This is the default value.</p></td>
</tr>
</tbody>
</table>

 

## Valid Passes


generalize

## Parent Hierarchy


[Microsoft-Windows-SharedAccess](microsoft-windows-sharedaccess.md) | **EnableICS**

## Applies To


For a list of the supported Windows editions and architectures that this component supports, see [Microsoft-Windows-SharedAccess](microsoft-windows-sharedaccess.md).

## XML Example


The following XML output shows how to set Shared Access.

``` syntax
<EnableICS>true</EnableICS>
<InternalIsBridge>true</InternalIsBridge>
<ExternalAdapter>MyExternalAdapter</ExternalAdapter>
```

## Related topics


[Microsoft-Windows-SharedAccess](microsoft-windows-sharedaccess.md)

[Microsoft-Windows-NetworkBridge](microsoft-windows-networkbridge-win7-microsoft-windows-networkbridge.md)

 

 

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20%5Bp_unattend\p_unattend%5D:%20EnableICS%20%20RELEASE:%20%2810/3/2016%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/default.aspx. "Send comments about this topic to Microsoft")





