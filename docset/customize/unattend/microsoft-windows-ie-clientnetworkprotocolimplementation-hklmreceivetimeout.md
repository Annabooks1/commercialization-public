---
title: HKLMReceiveTimeOut
description: HKLMReceiveTimeOut
MSHAttr:
- 'PreferredSiteName:MSDN'
- 'PreferredLib:/library/windows/hardware'
ms.assetid: eb04b5fd-ddc0-48c6-a1a4-2330b7b76fb1
ms.prod: W10
ms.mktglfcycl: deploy
ms.sitesec: msdn
---

# HKLMReceiveTimeOut


`HKLMReceiveTimeOut` specifies the number of milliseconds to wait for data to be received over the network for all users on the computer. This is also known as a socket receive.

## Values


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><em>Number_of_milliseconds</em></p></td>
<td><p>Specifies the number of milliseconds for data to be received over the network before timing out.</p>
<p>The default value is <strong>30000</strong> (30 seconds). <em>Number_of_milliseconds</em> is an integer from 5000 (five seconds) through 86400000 (one day).</p></td>
</tr>
</tbody>
</table>

 

## Valid Passes


oobeSystem

## Parent Hierarchy


[microsoft-windows-ie-clientnetworkprotocolimplementation-](microsoft-windows-ie-clientnetworkprotocolimplementation-.md) | **HKLMReceiveTimeOut**

## Applies To


For a list of the supported Windows editions and architectures that this component supports, see [microsoft-windows-ie-clientnetworkprotocolimplementation-](microsoft-windows-ie-clientnetworkprotocolimplementation-.md).

## XML Example


The following XML output shows how to set Internet Explorer to wait 45 seconds to receive a response to a request. If the response takes longer than this time-out value, the request is canceled.

``` syntax
<HKLMReceiveTimeOut>45000</HKLMReceiveTimeOut>
```

## Related topics


[microsoft-windows-ie-clientnetworkprotocolimplementation-](microsoft-windows-ie-clientnetworkprotocolimplementation-.md)

 

 

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20%5Bp_unattend\p_unattend%5D:%20HKLMReceiveTimeOut%20%20RELEASE:%20%2810/3/2016%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/default.aspx. "Send comments about this topic to Microsoft")





