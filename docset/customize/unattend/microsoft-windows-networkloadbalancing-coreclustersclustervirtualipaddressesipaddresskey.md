---
title: Key
description: Key
MSHAttr:
- 'PreferredSiteName:MSDN'
- 'PreferredLib:/library/windows/hardware'
ms.assetid: e8fc6113-3a14-47f0-8ab4-2baa1a23dfda
ms.prod: W10
ms.mktglfcycl: deploy
ms.sitesec: msdn
---

# Key


`Key` specifies the name of the virtual IP address. The name is specified as an attribute in the IP address.

**Note**  
-   This XML attribute does not appear in the **Properties** pane of Windows System Image Manager (Windows SIM) until you add an [IpAddress](microsoft-windows-networkloadbalancing-coreclustersclustervirtualipaddressesipaddress.md) to the answer file.

-   The value for `Key` is added to the answer file as an attribute of the [IpAddress](microsoft-windows-networkloadbalancing-coreclustersclustervirtualipaddressesipaddress.md) element. The attribute `wcm:keyValue` is used to identify each unique virtual IP Address. For example, you can specify three different virtual IP addresses by using the `Key` value of **Ip1**, **Ip2**, and **Ip3**.

 

## Values


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><em>Key</em></p></td>
<td><p>Specifies the name of the virtual IP address.</p></td>
</tr>
</tbody>
</table>

 

## Valid Passes


specialize

## Parent Hierarchy


[Microsoft-Windows-NetworkLoadBalancing-Core](microsoft-windows-networkloadbalancing-core.md) | [Clusters](microsoft-windows-networkloadbalancing-coreclusters.md) | [Cluster](microsoft-windows-networkloadbalancing-coreclusterscluster.md) | [VirtualIpAddresses](microsoft-windows-networkloadbalancing-coreclustersclustervirtualipaddresses.md) | [IpAddress](microsoft-windows-networkloadbalancing-coreclustersclustervirtualipaddressesipaddress.md) | **Key**

## Applies To


For a list of the supported Windows editions and architectures that this component supports, see [Microsoft-Windows-NetworkLoadBalancing-Core](microsoft-windows-networkloadbalancing-core-win7-microsoft-windows-networkloadbalancing-core.md).

## XML Example


The following XML output shows how to specify a virtual IP address by using the name "Ip1".

``` syntax
<IpAddress wcm:keyValue="Ip1">
   <IpAddress>10.192.45.1</IpAddress>
   <NetworkMask>255.255.255.0</NetworkMask>
</IpAddress>
```

## Related topics


[IpAddress](microsoft-windows-networkloadbalancing-coreclustersclustervirtualipaddressesipaddress.md)

 

 

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20%5Bp_unattend\p_unattend%5D:%20Key%20%20RELEASE:%20%2810/3/2016%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/default.aspx. "Send comments about this topic to Microsoft")





