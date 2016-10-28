---
title: IpAddress
description: IpAddress
MSHAttr:
- 'PreferredSiteName:MSDN'
- 'PreferredLib:/library/windows/hardware'
ms.assetid: 765b659c-d699-4e03-aa56-9d5ab028b85f
ms.prod: W10
ms.mktglfcycl: deploy
ms.sitesec: msdn
---

# IpAddress


`IpAddress` specifies details about a cluster's virtual IP address, not associated with the cluster. At least one IP Address setting must be specified.

**Note**  
To enable this Network Load Balancing setting, the NetworkLoadBalancingFullServer package must be enabled in the Windows image you are installing. To do this, use Windows System Image Manager to add the Microsoft-Windows-Foundation-Package to your answer file, and then configure the NetworkLoadBalancingFullServer package to enable it. For more information about adding and configuring packages, see the [Windows Assessment and Deployment (Windows ADK) Technical Reference](http://go.microsoft.com/fwlink/?LinkId=206587).

 

## Child Elements


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p>[Key](microsoft-windows-networkloadbalancing-core-clusters-clustervirtualipaddressesipaddresskey.md)</p></td>
<td><p>Specifies the name of the virtual IP address.</p>
<div class="alert">
<strong>Note</strong>  
<p>This XML attribute does not appear in the <strong>Properties</strong> pane of Windows System Image Manager (Windows SIM) until you add this IP Address to the answer file.</p>
</div>
<div>
 
</div></td>
</tr>
<tr class="even">
<td><p>[IpAddress](microsoft-windows-networkloadbalancing-core-clusters-clustervirtualipaddressesipaddressipaddress.md)</p></td>
<td><p>Specifies the IP address for the cluster's virtual IP address.</p></td>
</tr>
<tr class="odd">
<td><p>[NetworkMask](microsoft-windows-networkloadbalancing-core-clusters-clustervirtualipaddressesipaddressnetworkmask.md)</p></td>
<td><p>Specifies the network mask for the cluster's virtual IP address.</p></td>
</tr>
</tbody>
</table>

 

## Valid Passes


specialize

## Parent Hierarchy


[microsoft-windows-networkloadbalancing-core-](microsoft-windows-networkloadbalancing-core-.md) | [Clusters](microsoft-windows-networkloadbalancing-core-clusters.md) | [Cluster](microsoft-windows-networkloadbalancing-core-clusters-cluster.md) | [VirtualIpAddresses](microsoft-windows-networkloadbalancing-core-clusters-clustervirtualipaddresses.md) | **IPAddress**

## Applies To


For a list of the supported Windows editions and architectures that this component supports, see [microsoft-windows-networkloadbalancing-core-](microsoft-windows-networkloadbalancing-core--win7-microsoft-windows-networkloadbalancing-core-.md).

## XML Example


The following XML output specifies details about the cluster's virtual IP address.

``` syntax
<IpAddress wcm:keyValue="Ip1">
   <IpAddress>207.46.197.32</IpAddress>
   <NetworkMask>255.255.255.0</NetworkMask>
</IpAddress>
```

## Related topics


[VirtualIpAddresses](microsoft-windows-networkloadbalancing-core-clusters-clustervirtualipaddresses.md)

 

 

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20%5Bp_unattend\p_unattend%5D:%20IpAddress%20%20RELEASE:%20%2810/3/2016%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/default.aspx. "Send comments about this topic to Microsoft")





