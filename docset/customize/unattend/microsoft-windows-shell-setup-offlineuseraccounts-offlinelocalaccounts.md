---
title: OfflineLocalAccounts
description: OfflineLocalAccounts specifies offline local accounts to be created during installation.
MSHAttr:
- 'PreferredSiteName:MSDN'
- 'PreferredLib:/library/windows/hardware'
ms.assetid: 72A51941-7077-4646-BB6C-3CE075C36824
ms.prod: W10
ms.mktglfcycl: deploy
ms.sitesec: msdn
---

# OfflineLocalAccounts


`OfflineLocalAccounts` specifies offline local accounts to be created during installation.

You can use the **sysprep/generalize** command in conjunction with `OfflineLocalAccounts` to change account information. See the B[Best Practices for Authoring Answer Files](https://msdn.microsoft.com/library/windows/hardware/dn915073) topic for details.

## Child Elements


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p>[LocalAccount](microsoft-windows-shell-setup-offlineuseraccounts-offlinelocalaccounts-localaccount.md)</p></td>
<td><p>Specifies a local account to be created during installation.</p></td>
</tr>
</tbody>
</table>

 

## Valid Configuration Passes


offlineServicing

## Parent Hierarchy


[Microsoft-Windows-Shell-Setup](microsoft-windows-shell-setup.md)| [OfflineUserAccounts](microsoft-windows-shell-setup-offlineuseraccounts.md) | **OfflineLocalAccounts**

## Applies To


Windows 10 for desktop editions (Home, Pro, Enterprise, and Education)

Windows Server 2016

For a list of the Windows® editions and architectures that this component supports, see [Microsoft-Windows-Shell-Setup](microsoft-windows-shell-setup.md).

 

 

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20%5Bp_unattend\p_unattend%5D:%20OfflineLocalAccounts%20%20RELEASE:%20%2810/3/2016%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/default.aspx. "Send comments about this topic to Microsoft")




