---
title: HideAllBootUI
description: Suppresses all Windows UI elements (logo, status indicator, and status message) during startup.
MSHAttr:
- 'PreferredSiteName:MSDN'
- 'PreferredLib:/library/windows/hardware'
ms.assetid: B2BF86DC-163A-477C-A54B-4AACB5BC4DC3
ms.prod: W10
ms.mktglfcycl: deploy
ms.sitesec: msdn
ms.author: alhopper
ms.date: 05/02/2017
ms.topic: article
ms.prod: windows-hardware
ms.technology: windows-oem
---

# HideAllBootUI


Suppresses all Windows UI elements (logo, status indicator, and status message) during startup.

## Values


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Value</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p>0</p></td>
<td><p>Do not suppress Windows UI elements during startup.</p>
<p>This is the default value.</p></td>
</tr>
<tr class="even">
<td><p>1</p></td>
<td><p>Suppress Windows UI elements during startup.</p></td>
</tr>
</tbody>
</table>

 

## Parent Hierarchy


[Microsoft-Windows-Embedded-BootExp](microsoft-windows-embedded-bootexp.md) | **HideAllBootUI**

## Valid Configuration Passes


specialize

oobeSystem

## Applies To


For a list of the Windows editions and architectures that this component supports, see [Microsoft-Windows-Embedded-BootExp](microsoft-windows-embedded-bootexp.md).

## XML example


``` syntax
<settings pass="specialize">
    <component name="Microsoft-Windows-Embedded-BootExp" processorArchitecture="x86" publicKeyToken="31bf3856ad364e35" language="neutral" versionScope="nonSxS" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
      <HideAllBootUI>1</HideAllBootUI>
    </component>
</settings>
```

 

 

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20%5Bp_unattend\p_unattend%5D:%20HideAllBootUI%20%20RELEASE:%20%2810/3/2016%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/default.aspx. "Send comments about this topic to Microsoft")




