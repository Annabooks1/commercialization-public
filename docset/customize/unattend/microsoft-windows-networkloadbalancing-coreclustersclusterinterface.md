---
title: Interface
description: Interface
MSHAttr:
- 'PreferredSiteName:MSDN'
- 'PreferredLib:/library/windows/hardware'
ms.assetid: 1e238012-ca6c-454a-b36a-26156d041b55
ms.prod: W10
ms.mktglfcycl: deploy
ms.sitesec: msdn
---

# Interface


`Interface` specifies the interface name or interface MAC address that you bind to Network Load Balancing. This is a required setting.

**Note**  
To enable this Network Load Balancing setting, the NetworkLoadBalancingFullServer package must be enabled in the Windows® image you are installing. To do this, use Windows System Image Manager to add the Microsoft-Windows-Foundation-Package to your answer file, and then configure the NetworkLoadBalancingFullServer package to enable it. For more information about adding and configuring packages, see the [Windows® Assessment and Deployment (Windows ADK) Technical Reference](http://go.microsoft.com/fwlink/?LinkId=206587).

 

## Values


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><em>Interface</em></p></td>
<td><p>Specifies the name of the interface or the interface MAC address.</p></td>
</tr>
</tbody>
</table>

 

This string type does not support empty elements. Do not create an empty value for this setting.

## Valid Passes


specialize

## Parent Hierarchy


[Microsoft-Windows-NetworkLoadBalancing-Core](microsoft-windows-networkloadbalancing-core.md) | [Clusters](microsoft-windows-networkloadbalancing-coreclusters.md) | [Cluster](microsoft-windows-networkloadbalancing-coreclusterscluster.md) | **Interface**

## Applies To


For a list of the supported Windows® editions and architectures that this component supports, see [Microsoft-Windows-NetworkLoadBalancing-Core](microsoft-windows-networkloadbalancing-core-win7-microsoft-windows-networkloadbalancing-core.md).

## XML Example


The following XML output specifies that the interface to be used is Local Area Connection 2.

``` syntax
<Interface>Local Area Connection 2</Interface>
```

The following XML output specifies the interface to be used by the MAC address.

``` syntax
<Interface>00-30-6E-12-9F-5E</Interface>
```

## Related topics


[Cluster](microsoft-windows-networkloadbalancing-coreclusterscluster.md)

 

 

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20%5Bp_unattend\p_unattend%5D:%20Interface%20%20RELEASE:%20%2810/3/2016%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/default.aspx. "Send comments about this topic to Microsoft")





