---
title: UninstallWindowsRE
description: UninstallWindowsRE
MSHAttr:
- 'PreferredSiteName:MSDN'
- 'PreferredLib:/library/windows/hardware'
ms.assetid: 4118d371-d469-4d26-bb1a-a5540f31feb2
ms.prod: W10
ms.mktglfcycl: deploy
ms.sitesec: msdn
---

# UninstallWindowsRE


`UninstallWindowsRE` specifies whether Windows Recovery Environment (Windows RE) is installed or removed from the system.

You can save hard disk space by configuring Windows Setup to uninstall Windows RE from the local hard disk.

**Warning**  
We recommend that you do not use this setting. Uninstalling Windows RE disables functionalities that allow users to troubleshoot and recover from startup problems.

 

## Values


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><strong>true</strong></p></td>
<td><p>When Windows Setup completes, any default or OEM-specified Windows RE image is deleted from the local hard disk.</p></td>
</tr>
<tr class="even">
<td><p><strong>false</strong></p></td>
<td><p>Specifies that when Windows Setup completes, any default or OEM-specified Windows RE image (including the default image) is installed on the local hard disk.</p>
<p>This is the default value.</p></td>
</tr>
</tbody>
</table>

 

## Valid Configuration Passes


oobeSystem

## Parent Hierarchy


[Microsoft-Windows-WinRE-RecoveryAgent](microsoft-windows-winre-recoveryagent.md) | **UninstallWindowsRE**

## Applies To


For the list of the Windows editions and architectures that this component supports, see [Microsoft-Windows-WinRE-RecoveryAgent](microsoft-windows-winre-recoveryagent.md).

## XML Example


The following XML output shows how to instruct Windows to save drive space by uninstalling any default or OEM-specified Windows RE image from the system.

``` syntax
<UninstallWindowsRE>true</UninstallWindowsRE>
```

## Related topics


[Microsoft-Windows-WinRE-RecoveryAgent](microsoft-windows-winre-recoveryagent.md)

 

 

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20%5Bp_unattend\p_unattend%5D:%20UninstallWindowsRE%20%20RELEASE:%20%2810/3/2016%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/default.aspx. "Send comments about this topic to Microsoft")





