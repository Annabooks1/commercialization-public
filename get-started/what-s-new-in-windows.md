---
title: What's new in Windows 10, version 1709
description: New features for Windows 10, version 1709
ms.assetid: 1E8F0E54-1E5B-495B-848D-260620C7DF4F
ms.author: alhopper
ms.date: 10/17/2017
ms.topic: article
ms.prod: windows-hardware
ms.technology: windows-oem
---
# What's new in Windows 10, version 1709

Welcome to Windows 10, version 1709! Here are some resources to get you acquainted with the new features and changes introduced in this version of Windows 10.

## New in Design

### New hardware compatibility specifications

The Windows Hardware Compatibility Program is designed to help your company deliver systems, software, and hardware products that are compatible with Windows and run reliably on Windows 10 and Windows Server 2016. Systems are required to use components which have also passed compatibility testing. [Learn more >>](https://docs.microsoft.com/en-us/windows-hardware/design/compatibility/1709)

The following requirements are new for Windows 10, version 1709:

* [Device.DevFund.UniversalDriver](https://docs.microsoft.com/en-us/windows-hardware/design/compatibility/1709/device-devfund#Device.DevFund.UniversalDriver)
* [System.Fundamentals.Security](https://docs.microsoft.com/en-us/windows-hardware/design/compatibility/1709/systems#systemfundamentalssecurity)
* [System.Client.SensorCamera](https://docs.microsoft.com/en-us/windows-hardware/design/compatibility/1709/systems#systemclientsensorcamera)
* [System.Fundamentals.Firmware.HSTI](https://docs.microsoft.com/en-us/windows-hardware/design/compatibility/1709/systems#systemfundamentalsfirmware)

### New security guidelines

For this release, we’ve consolidated, reviewed, and updated the Windows security content for partner OEMs. There are topics on UEFI, TPM, and VBS requirements; topics on Windows Defender Device Guard, Windows Defender Application Guard, and Windows Defender Credential Guard; a topic on Secure Boot. [Learn more >>](https://docs.microsoft.com/en-us/windows-hardware/design/device-experiences/oem-security-considerations)

## New Customization options

### Customize the Get Help app

The Get Help app empowers customers to self-help with troubleshooters, instant answers, Microsoft support articles, and more, before contacting assisted support.

If you have a support app or support website you would like to direct customers towards, you can use unattend.xml to display your support option within the Get Help app. A link to your support app or website is surfaced wherever options to contact support are shown in the Get Help app. The first item in the list will be the link you provided. [Learn more >>](https://docs.microsoft.com/en-us/windows-hardware/customize/desktop/customize-get-help-app)

### Customize the Windows power slider

The new Windows performance power slider enables end customers to quickly and intelligently trade performance of their system for longer battery life. As a customer switches between the four slider modes to trade performance for battery life (or vice versa), Windows power settings are engaged behind the scenes. You are able to customize the default slider mode for both AC and DC, and can also configure the power settings, and PPM options, that are engaged for each slider mode. [Learn more >>](https://docs.microsoft.com/en-us/windows-hardware/customize/desktop/customize-power-slider)

## New in Manufacturing

### Updated Windows Full Flash Update (FFU) tool

[Learn more >>](https://docs.microsoft.com/en-us/windows-hardware/manufacture/desktop/deploy-windows-using-full-flash-update--ffu)

## New in Driver development

See [What's new in Driver development](https://docs.microsoft.com/en-us/windows-hardware/drivers/what-s-new-in-driver-development) for an in-depth look.

### Guidance for Universal Windows drivers

You can write a single driver that works on OneCoreUAP-based editions of Windows, such as Windows 10 for desktop editions (Home, Pro, Enterprise, and Education), Windows 10 Mobile, and Windows 10 IoT Core (IoT Core). Such a driver is called a Universal Windows driver. A Universal Windows driver calls a subset of the interfaces that are available to a Windows driver. [Learn more >>](https://msdn.microsoft.com/windows-drivers/develop/getting_started_with_universal_drivers)

### Update device firmware using Windows Update

You can update a removable or in-chassis device's firmware using the Windows Update (WU) service. To do this, you'll provide an update mechanism, implemented as a device driver, that includes the firmware payload. If your device uses a vendor-supplied driver, you have the option of adding the firmware update logic and payload to your existing function driver, or providing a separate firmware update driver package. [Learn more >>](https://docs.microsoft.com/en-us/windows-hardware/drivers/install/updating-device-firmware-using-windows-update)

### New Driver Package INF Registry Conversion Tool (reg2inf.exe)

The Driver Package INF Registry Conversion Tool (reg2inf.exe) tool converts a registry key and its values or a COM .dll implementing a DllRegisterServer routine into a set of INF AddReg directives for inclusion into a driver package INF file. This tool is particularly useful for converting existing INF RegisterDlls directives into INF AddReg directives in order to make an INF file universal. For more info about universal INF files, see Using a Universal INF File. [Learn more >>](https://docs.microsoft.com/en-us/windows-hardware/drivers/devtest/reg2inf)

### Debug using the new WinDbg Preview

WinDbg Preview is a brand-new version of the Windows debugger. With more modern visuals, faster windows, and a full-fledged scripting experience, WinDbg Preview builds on the extensible debugger data model and relies on the same engine as today’s WinDbg. Use all the commands, extensions, and workflows just like before. Great new features include Time Travel Debugging (TTD), which records the execution of an app or process, replays it both forwards and backwards, and uses queries to search through the entire trace. You can go back in time to better understand the conditions that lead up to the bug or replay the events multiple times to learn how best to fix a problem. [Learn more >>](https://docs.microsoft.com/en-us/windows-hardware/drivers/debugger/debugging-using-windbg-preview)