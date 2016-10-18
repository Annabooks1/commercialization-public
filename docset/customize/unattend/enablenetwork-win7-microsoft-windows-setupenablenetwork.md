---
title: EnableNetwork
description: EnableNetwork
MSHAttr:
- 'PreferredSiteName:MSDN'
- 'PreferredLib:/library/windows/hardware'
ms.assetid: ecffdab9-99bd-4e85-9bde-6505a341c7ec
ms.prod: W10
ms.mktglfcycl: deploy
ms.sitesec: msdn
---

# EnableNetwork


`EnableNetwork` specifies whether network connection is enabled. This setting applies only to Windows® Preinstallation Environment (Windows PE).

If you set `EnableNetwork` to **false**, network initialization is skipped, and any network settings are ignored.

In OEM, independent software vendor, or other customized Windows PE scenarios, the default value for `EnableNetwork` is **true**. In Windows Setup scenarios, the default value is **false**.

## Values


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><strong>true</strong></p></td>
<td><p>Specifies that network connection is enabled.</p></td>
</tr>
<tr class="even">
<td><p><strong>false</strong></p></td>
<td><p>Specifies that network connection is not enabled.</p></td>
</tr>
</tbody>
</table>

 

## Valid Passes


windowsPE

## Parent Hierarchy


[Microsoft-Windows-Setup](microsoft-windows-setup-win7-microsoft-windows-setup.md) | **EnableNetwork**

## Applies To


For a list of the supported Windows editions and architectures that this component supports, see [Microsoft-Windows-Setup](microsoft-windows-setup-win7-microsoft-windows-setup.md).

## XML Example


The following XML output shows how to disable network connection.

``` syntax
<EnableNetwork>false</EnableNetwork>
```

## Related topics


[Microsoft-Windows-Setup](microsoft-windows-setup-win7-microsoft-windows-setup.md)

 

 

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20%5Bp_unattend\p_unattend%5D:%20EnableNetwork%20%20RELEASE:%20%2810/3/2016%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/default.aspx. "Send comments about this topic to Microsoft")





