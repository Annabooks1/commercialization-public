---
title: Extend
description: Extend
MSHAttr:
- 'PreferredSiteName:MSDN'
- 'PreferredLib:/library/windows/hardware'
ms.assetid: 24b1b2c1-26e7-4d1b-8b09-8f0b11499e16
ms.prod: W10
ms.mktglfcycl: deploy
ms.sitesec: msdn
---

# Extend


`Extend` indicates whether to extend the partition to fill the remaining space on the hard disk. If this setting and [Size](size-win7-microsoft-windows-deploymentextendospartitionsize.md) are present in the same configuration pass, an error is logged, and installation is terminated.

## Values


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><strong>true</strong></p></td>
<td><p>Specifies that the partition is extended to fill the remaining space on the disk.</p></td>
</tr>
<tr class="even">
<td><p><strong>false</strong></p></td>
<td><p>Specifies that the partition is not extended. This is the default value.</p></td>
</tr>
</tbody>
</table>

 

**Note**  
You can extend only NTFS file-system partitions.

 

## Valid Passes


auditSystem

generalize

oobeSystem

specialize

## Parent Hierarchy


[Microsoft-Windows-Deployment](microsoft-windows-deployment-win7-microsoft-windows-deployment.md) | [ExtendOSPartition](extendospartition-win7-microsoft-windows-deploymentextendospartition.md) | **Extend**

## Applies To


For a list of the supported Windows® editions and architectures that this component supports, see [Microsoft-Windows-Deployment](microsoft-windows-deployment-win7-microsoft-windows-deployment.md).

## XML Example


The following XML output shows a deployment with no asynchronous or synchronous commands.

``` syntax
<AuditComputerName>
   <MustReboot>true</MustReboot>
   <Name>MyComputer</Name>
</AuditComputerName>
<ExtendOSPartition>
   <Extend>true</Extend>
</ExtendOSPartition>
<Reseal>
   <ForceShutdownNow>true</ForceShutdownNow>
   <Mode>Audit</Mode>
</Reseal>
```

## Related topics


[ExtendOSPartition](extendospartition-win7-microsoft-windows-deploymentextendospartition.md)

 

 

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20%5Bp_unattend\p_unattend%5D:%20Extend%20%20RELEASE:%20%2810/3/2016%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/default.aspx. "Send comments about this topic to Microsoft")





