---
title: microsoft-windows-pnpcustomizationswinpe-
description: microsoft-windows-pnpcustomizationswinpe-
MSHAttr:
- 'PreferredSiteName:MSDN'
- 'PreferredLib:/library/windows/hardware'
ms.assetid: 7be7b298-fba8-4adf-8880-d3277c26cb61
ms.prod: W10
ms.mktglfcycl: deploy
ms.sitesec: msdn
ms.author: alhopper
ms.date: 05/02/2017
ms.topic: article
ms.prod: windows-hardware
ms.technology: windows-oem
---

# microsoft-windows-pnpcustomizationswinpe-


The microsoft-windows-pnpcustomizationswinpe- component is used to add one or more out-of-box drivers to a Windows installation. Drivers that are located in the path specified by [DriverPaths](microsoft-windows-pnpcustomizationswinpe-driverpaths.md) are copied to the driver store of the Windows installation during the windowsPE configuration pass.

You can add boot-critical as well as non boot-critical drivers with this component to a Windows image before it is installed.

## In This Section


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p>[DriverPaths](microsoft-windows-pnpcustomizationswinpe-driverpaths.md)</p></td>
<td><p>Specifies one or more driver paths that contain out-of-box drivers. Drivers in this path are copied to the Windows image during the <strong>windowsPE</strong> configuration pass.</p></td>
</tr>
</tbody>
</table>

 

## Applies To


To determine whether a component applies to the image you’re building, load your image into Windows SIM and search for the component or setting name. For information on how to view components and settings, see [Configure Components and Settings in an Answer File](https://msdn.microsoft.com/library/windows/hardware/dn915078).

## Related topics


[Components](components-b-unattend.md)

[Microsoft-Windows-PnpCustomizationsNonWinPE](microsoft-windows-pnpcustomizationsnonwinpe.md)

 

 







