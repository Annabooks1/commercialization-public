---
title: fDenyTSConnections
description: fDenyTSConnections
MSHAttr:
- 'PreferredSiteName:MSDN'
- 'PreferredLib:/library/windows/hardware'
ms.assetid: ca7b2f3e-d1a2-4077-a9e9-8d6c2e7233c1
ms.prod: W10
ms.mktglfcycl: deploy
ms.sitesec: msdn
---

# fDenyTSConnections


`fDenyTSConnections` specifies whether Remote Desktop connections are enabled.

There are several settings that must be configured to enable Remote Desktop connections during an unattended installation. First, you must enable Remote Desktop connections by using the `fDenyTSConnections` setting. You must also enable the Remote Desktop group in Windows Firewall. For more information, see "Enable Remote Desktop" in the Windows Assessment and Deployment Kit (Windows ADK).

## Values


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><strong>true</strong></p></td>
<td><p>Specifies that remote desktop connections are denied. This is the default value.</p></td>
</tr>
<tr class="even">
<td><p><strong>false</strong></p></td>
<td><p>Specifies that remote desktop connections are enabled.</p></td>
</tr>
</tbody>
</table>

 

## Valid Passes


offlineServicing

generalize

specialize

## Parent Hierarchy


[Microsoft-Windows-TerminalServices-LocalSessionManager]microsoft-windows-terminalservices-localsessionmanager.md) | **fDenyTSConnections**

## Applies To


For a list of the supported Windows® editions and architectures that this component supports, see [Microsoft-Windows-TerminalServices-LocalSessionManager](microsoft-windows-terminalservices-localsessionmanager-win7-microsoft-windows-terminalservices-localsessionmanager.md).

## XML Example


The following XML output shows how to set this element so that remote terminal service connections are enabled.

``` syntax
<fDenyTSConnections>false</fDenyTSConnections>
```

## Related topics


[Microsoft-Windows-TerminalServices-LocalSessionManager](microsoft-windows-terminalservices-localsessionmanager-win7-microsoft-windows-terminalservices-localsessionmanager.md)

 

 

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20%5Bp_unattend\p_unattend%5D:%20fDenyTSConnections%20%20RELEASE:%20%2810/3/2016%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/default.aspx. "Send comments about this topic to Microsoft")





