---
title: Microsoft-Windows-Shell-Setup
description: Microsoft-Windows-Shell-Setup
MSHAttr:
- 'PreferredSiteName:MSDN'
- 'PreferredLib:/library/windows/hardware'
ms.assetid: eeac1b17-6ef9-4ba6-9888-7adf9387ec04
ms.mktglfcycl: deploy
ms.sitesec: msdn
ms.author: alhopper
ms.date: 05/02/2017
ms.topic: article
ms.prod: windows-hardware
ms.technology: windows-oem
---

# Microsoft-Windows-Shell-Setup


Microsoft-Windows-Shell-Setup contains elements and settings that control how the Windows operating system shell is installed on a destination computer.

## In This Section


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p>[AutoLogon](microsoft-windows-shell-setup-autologon.md)</p></td>
<td><p>Specifies credentials for an account that is used to automatically log on to the computer.</p></td>
</tr>
<tr class="even">
<td><p>[BluetoothTaskbarIconEnabled](microsoft-windows-shell-setup-bluetoothtaskbariconenabled.md)</p></td>
<td><p>Specifies whether to enable the Bluetooth taskbar icon.</p></td>
</tr>
<tr class="odd">
<td><p>[ComputerName](microsoft-windows-shell-setup-computername.md)</p></td>
<td><p>Specifies the name of the computer.</p></td>
</tr>
<tr class="even">
<td><p>[ConvertibleSlateModePromptPreference](microsoft-windows-shell-setup-convertibleslatemodepromptpreference.md)</p></td>
<td><p>Configure to support prompts triggered by changes to [ConvertibleSlateMode](microsoft-windows-gpiobuttons-convertibleslatemode.md). OEMs must make sure that <code>ConvertibleSlateMode</code> is always accurate for their devices.</p></td>
</tr>
<tr class="odd">
<td><p>[CopyProfile](microsoft-windows-shell-setup-copyprofile.md)</p></td>
<td><p>Specifies whether the default user profile that is normally stored in the C:\Users\Default User folder is overwritten by copying the current user's profile.</p></td>
</tr>
<tr class="even">
<td><p>[DisableAutoDaylightTimeSet](microsoft-windows-shell-setup-disableautodaylighttimeset.md)</p></td>
<td><p>Specifies whether to enable the destination computer to automatically change between daylight saving time and standard time.</p></td>
</tr>
<tr class="odd">
<td><p>[Display](microsoft-windows-shell-setup-display.md)</p></td>
<td><p>Specifies display settings to apply to a destination computer.</p></td>
</tr>
<tr class="even">
<td><p>[FirstLogonCommands](microsoft-windows-shell-setup-firstlogoncommands.md)</p></td>
<td><p>Specifies commands to run the first time that an end user logs on to the computer.</p></td>
</tr>
<tr class="odd">
<td><p>[FolderLocations](microsoft-windows-shell-setup-folderlocations.md)</p></td>
<td><p>Specifies the location of the user profile and program data folders.</p>
<div class="alert">
<strong>Important</strong>  
<p>This setting should be used only in a test environment. If you change the default location of the user profile directories or program data folders to a volume other than the system volume, you cannot service your image.</p>
</div>
<div>
 
</div></td>
</tr>
<tr class="even">
<td><p>[LogonCommands](microsoft-windows-shell-setup-logoncommands.md)</p></td>
<td><p>Specifies commands to run when an end user logs on to the computer.</p></td>
</tr>
<tr class="odd">
<td><p>[NotificationArea](microsoft-windows-shell-setup-notificationarea.md)</p></td>
<td><p>Specifies settings that are related to the system notification area at the far right of the taskbar.</p></td>
</tr>
<tr class="even">
<td><p>[OEMInformation](microsoft-windows-shell-setup-oeminformation.md)</p></td>
<td><p>Specifies information about the OEM, including the name, the model of the computer, and a logo for the OEM.</p></td>
</tr>
<tr class="odd">
<td><p>[OEMName](microsoft-windows-shell-setup-oemname.md)</p></td>
<td><p>Specifies the name of the OEM for the group or groups of app tiles that you pin to the Start screen.</p></td>
</tr>
<tr class="even">
<td><p>[OfflineUserAccounts](microsoft-windows-shell-setup-offlineuseraccounts.md)</p></td>
<td><p>Specifies local accounts to be created, domain accounts to be added, and the administrator password.</p></td>
</tr>
<tr class="odd">
<td><p>[OOBE](microsoft-windows-shell-setup-oobe.md)</p></td>
<td><p>Specifies values that suppress certain pages of OOBE.</p></td>
</tr>
<tr class="even">
<td><p>[ProductKey](microsoft-windows-shell-setup-productkey.md)</p></td>
<td><p>Specifies the product key for the Windows edition.</p></td>
</tr>
<tr class="odd">
<td><p>[RegisteredOrganization](microsoft-windows-shell-setup-registeredorganization.md)</p></td>
<td><p>Specifies information about the computer's owner.</p></td>
</tr>
<tr class="even">
<td><p>[RegisteredOwner](microsoft-windows-shell-setup-registeredowner.md)</p></td>
<td><p>Specifies information about the organization of the computer's owner.</p></td>
</tr>
<tr class="odd">
<td><p>[ShowPowerButtonOnStartScreen](microsoft-windows-shell-setup-showpowerbuttononstartscreen.md)</p></td>
<td><p>Specifies that the <strong>Power Options</strong> button is visible on the Start screen.</p></td>
</tr>
<tr class="even">
<td><p>[SignInMode](microsoft-windows-shell-setup-signinmode.md)</p></td>
<td><p>Specifies whether users switch to tablet mode by default after signing in.</p></td>
</tr>
<tr class="odd">
<td><p>[StartTiles](microsoft-windows-shell-setup-starttiles.md)</p></td>
<td><p>Specifies the position of up to 24 app tiles on the <strong>Start</strong> screen, and one app badge on the <strong>Lock</strong> screen.</p></td>
</tr>
<tr class="even">
<td><p>[TaskbarLinks](microsoft-windows-shell-setup-taskbarlinks.md)</p></td>
<td><p>Specifies shortcuts to display on the taskbar. You can specify up to three links.</p></td>
</tr>
<tr class="odd">
<td><p>[Themes](microsoft-windows-shell-setup-themes.md)</p></td>
<td><p>Specifies custom elements of the Windows visual style.</p></td>
</tr>
<tr class="even">
<td><p>[TimeZone](microsoft-windows-shell-setup-timezone.md)</p></td>
<td><p>Specifies the computer's time zone.</p></td>
</tr>
<tr class="odd">
<td><p>[UserAccounts](microsoft-windows-shell-setup-useraccounts.md)</p></td>
<td><p>Specifies local accounts to be created or domain accounts to be added during installation.</p></td>
</tr>
<tr class="even">
<td><p>[VisualEffects](microsoft-windows-shell-setup-visualeffects.md)</p></td>
<td><p>Specifies additional display settings.</p></td>
</tr>
<tr class="odd">
<td><p>[WindowsFeatures](microsoft-windows-shell-setup-windowsfeatures.md)</p></td>
<td><p>Specifies whether to show entry points for Internet Explorer, Media Center, and Windows Media Player.</p></td>
</tr>
</tbody>
</table>

 

## Applies To


To determine whether a component applies to the image you’re building, load your image into Windows SIM and search for the component or setting name. For information on how to view components and settings, see [Configure Components and Settings in an Answer File](https://docs.microsoft.com/en-us/windows-hardware/customize/desktop/wsim/configure-components-and-settings-in-an-answer-file).

## Related topics


[Components](components-b-unattend.md)

 

 







