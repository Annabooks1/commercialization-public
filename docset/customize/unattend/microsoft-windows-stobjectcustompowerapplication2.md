---
title: CustomPowerApplication2
description: CustomPowerApplication2
MSHAttr:
- 'PreferredSiteName:MSDN'
- 'PreferredLib:/library/windows/hardware'
ms.assetid: 88677e57-8acd-46df-9560-467e376b6652
ms.prod: W10
ms.mktglfcycl: deploy
ms.sitesec: msdn
---

# CustomPowerApplication2


`CustomPowerApplication2` specifies the second Battery Meter customized context menu item.

## Child Elements


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p>[Application](microsoft-windows-stobjectcustompowerapplication2application.md)</p></td>
<td><p>Specifies the name and the path of the application to run.</p></td>
</tr>
<tr class="even">
<td><p>[IconID](microsoft-windows-stobjectcustompowerapplication2iconid.md)</p></td>
<td><p>Specifies the optional icon resource ID.</p></td>
</tr>
<tr class="odd">
<td><p>[ItemName](microsoft-windows-stobjectcustompowerapplication2itemname.md)</p></td>
<td><p>Specifies the display text of the application.</p></td>
</tr>
<tr class="even">
<td><p>[Parameters](microsoft-windows-stobjectcustompowerapplication2parameters.md)</p></td>
<td><p>Specifies the optional parameters to use when running the application.</p></td>
</tr>
</tbody>
</table>

 

## Valid Passes


generalize

specialize

## Parent Hierarchy


[Microsoft-Windows-stobject](microsoft-windows-stobject.md) | **CustomPowerApplication2**

## Applies To


For the list of the supported Windows editions and architectures that this component supports, see [Microsoft-Windows-stobject](microsoft-windows-stobject.md).

## XML Example


The following XML output specifies how to configure `CustomPowerApplication2`.

``` syntax
<CustomPowerApplication2>
   <Application>C:\Program Files\CustomPower\Application.exe</Application> 
   <IconID>@%ProgramFiles%\Microsoft Shared\Resource.dll,-200</IconID> 
   <ItemName>%ProgramFiles%\Microsoft Shared\Resource.dll,-100</ItemName> 
   <Parameters>-param</Parameters> 
</CustomPowerApplication2>
```

## Related topics


[Microsoft-Windows-stobject](microsoft-windows-stobject.md)

 

 

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20%5Bp_unattend\p_unattend%5D:%20CustomPowerApplication2%20%20RELEASE:%20%2810/3/2016%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/default.aspx. "Send comments about this topic to Microsoft")





