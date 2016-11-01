---
title: ScreenSaver
description: ScreenSaver
MSHAttr:
- 'PreferredSiteName:MSDN'
- 'PreferredLib:/library/windows/hardware'
ms.assetid: 49a2e156-f277-4f3b-9d92-d630bb510143
ms.prod: W10
ms.mktglfcycl: deploy
ms.sitesec: msdn
---

# ScreenSaver


In Windows 10 version 1607, ScreenSaver is deprecated.

`ScreenSaver` specifies the path to a Windows screen saver file in a theme.

**Note**  
We do not recommend setting this value. Instead, we recommend using automatic power plans to dim the screen. This can help reduce system power consumption. For more information, see [Understanding Battery Life and Power Plans](http://go.microsoft.com/fwlink/p/?linkid=208183) in the Windows Assessment and Deployment Kit (Windows ADK).

 

## Values


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><em>Screen_saver_file</em></p></td>
<td><p>Specifies the name of the screen saver file. <em>Screen_saver_file</em> is a string with a maximum length of 256 characters.</p></td>
</tr>
</tbody>
</table>

 

## Valid Configuration Passes


specialize

auditSystem

auditUser

oobeSystem

## Parent Hierarchy


[Microsoft-Windows-Shell-Setup](microsoft-windows-shell-setup.md) | [Themes](microsoft-windows-shell-setup-themes.md) | **ScreenSaver**

## Applies To


For a list of the Windows editions and architectures that this component supports, see [Microsoft-Windows-Shell-Setup](microsoft-windows-shell-setup.md).

## Related topics


[Themes](microsoft-windows-shell-setup-themes.md)

 

 

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20%5Bp_unattend\p_unattend%5D:%20ScreenSaver%20%20RELEASE:%20%2810/3/2016%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/default.aspx. "Send comments about this topic to Microsoft")





