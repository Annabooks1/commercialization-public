---
title: What's new in the Windows ADK and ADK tools
description: What's new in Windows ADK and ADK tools
Search.SourceType: Video
ms.assetid: EE27ABF7-C197-4E8E-AC1B-77266E2B9FD9
---

# What's new in ADK kits and tools

## <a href="" id="adk"></a>What’s new in the the Windows ADK for Windows 10, version 1607

### Pick and choose desktop applications

With [siloed provisioning packages](manufacture\desktop\siloed-provisioning-packages.md), you can now pick and choose which desktop applications to add to your images during deployment. You no longer need to recapture the entire set of applications into your recovery image, they’re added in automatically. These packages support space-saving features like Compact OS and single-instancing. 

### Build IoT Core images for large-scale deployment

Capture your apps, drivers, and settings, and deploy them securely to new devices. Learn how with the [IoT Core manufacturing guides](manufacture\iot\iot-core-manufacturing-guide.md).

### The Chinese (Hong Kong SAR) language pack (zh-HK) is no longer used.

The Chinese (Taiwan) language pack (zh-TW) supports both Taiwan and Hong Kong locales. For more information, see Available Language Packs for Windows.

### More changes
See [What's new in Design](https://msdn.microsoft.com/library/windows/hardware/mt703371.aspx), [Change history for customization docs](https://msdn.microsoft.com/en-us/library/windows/hardware/mt723363(v=vs.85).aspx), [What's new in manufacturing](manufacture/whats-new-in-windows-manufacturing.md), and [Changed answer file settings for desktop editions](https://msdn.microsoft.com/library/windows/hardware/mt750416.aspx)</li>

## <a href="" id="adk"></a>What’s new in the Windows ADK, version 1511

The Windows ADK now includes [Windows Imaging and Configuration Designer](p_icd.icd_portal), the [Windows Assessment Toolkit](p_assessments.windows_assessment_toolkit), the [Windows Performance Toolkit](p_wpt.windows_performance_toolkit), and several new and improved deployment tools that can help you automate a large-scale deployment of Windows 10.

### Windows Imaging and Configuration Designer (ICD)

-   Quickly create a provisioning package that you can use to customize devices without re-imaging.
-   Build a customized Windows 10 image for specific market segments and regions.

See [Getting started with Windows ICD](p_icd.getting_started_with_the_imaging_configuration_and_designer_tool) for more information.

### Push-button reset incorporates system updates by default

Users can now refresh or restore their PCs to the updated version of the system files, instead of having to reinstall each update individually.

### Partial language packs now available

Want to add more languages for users when they turn on their device? Instead of adding full language packs, save space by adding just the base user interface files for a language. Later, if your user needs handwriting or voice recognition capabilities, Windows can download them as needed.

For more information, see [Language Packs (lp.cab)](p_adk_online.language_packs__lpcab__and_windows_deployment).

### New package type: Capabilities

This new Windows package type lets you request services like Microsoft .NET or languages without specifying the version. Use the DISM tool to search multiple sources like Windows Update or your corporate servers to find and install the latest version.

### Save space by running Windows from compressed OS files

You can now run Windows directly from compressed files. This is similar to WIMBoot, introduced in Windows 8.1 Update 1. This new process uses individual files instead of a static WIM file. When updating system files, Windows now replaces the old files instead of keeping both copies.


## Related topics

- [Kits and tools overview](kit-and-tools-overview.md)

- [What's new in driver development](what-s-new-in-driver-development.md)

- [What's new in the Windows Performance Toolkit](https://msdn.microsoft.com/en-us/library/windows/hardware/dn927303(v=vs.85).aspx)

- [What's new in the Hardware Lab Kit](https://msdn.microsoft.com/library/windows/hardware/mt187880.aspx)
 

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20%5Bp_getstarted\p_getstarted%5D:%20What's%20new%20in%20kits%20and%20tools%20%20RELEASE:%20%286/15/2016%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/default.aspx. "Send comments about this topic to Microsoft")





