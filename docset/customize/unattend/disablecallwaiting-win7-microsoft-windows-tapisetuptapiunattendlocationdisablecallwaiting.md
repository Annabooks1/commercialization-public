---
title: DisableCallWaiting
description: DisableCallWaiting
MSHAttr:
- 'PreferredSiteName:MSDN'
- 'PreferredLib:/library/windows/hardware'
ms.assetid: 2eb91368-8eaf-467b-bdaa-713d57986b9a
ms.prod: W10
ms.mktglfcycl: deploy
ms.sitesec: msdn
---

# DisableCallWaiting


`DisableCallWaiting` specifies the number to dial for disabling call waiting.

## Values


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><em>Number_to_dial</em></p></td>
<td><p>Specifies the number to dial. Valid values are the digits <strong>0</strong> through <strong>9</strong>. <em>Number_to_dial</em> is a string.</p></td>
</tr>
</tbody>
</table>

 

This string type supports empty elements.

## Valid Passes


specialize

## Parent Hierarchy


[Microsoft-Windows-TapiSetup](microsoft-windows-tapisetup-win7-microsoft-windows-tapisetup.md) | [TapiUnattendLocation](tapiunattendlocation-win7-microsoft-windows-tapisetuptapiunattendlocation.md) | **DisableCallWaiting**

## Applies To


For a list of the supported Windows® editions and architectures that this component supports, see [Microsoft-Windows-TapiSetup](microsoft-windows-tapisetup-win7-microsoft-windows-tapisetup.md).

## XML Example


The following XML output shows how to set the location from which you are calling.

``` syntax
<TapiUnattendLocation>
   <AreaCode>123</AreaCode>
   <CountryOrRegion>123</CountryOrRegion>
   <DisableCallWaiting>7</DisableCallWaiting>
   <InternationalCarrierCode>123456789</InternationalCarrierCode>
   <LongDistanceAccess>11</LongDistanceAccess>
   <LongDistanceCarrierCode>123456789</LongDistanceCarrierCode>
   <Name>MyLocation</Name>
   <OutsideAccess>9</OutsideAccess>
   <PulseOrToneDialing>1</PulseOrToneDialing>
</TapiUnattendLocation>
```

## Related topics


[TapiUnattendLocation](tapiunattendlocation-win7-microsoft-windows-tapisetuptapiunattendlocation.md)

 

 

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20%5Bp_unattend\p_unattend%5D:%20DisableCallWaiting%20%20RELEASE:%20%2810/3/2016%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/default.aspx. "Send comments about this topic to Microsoft")





