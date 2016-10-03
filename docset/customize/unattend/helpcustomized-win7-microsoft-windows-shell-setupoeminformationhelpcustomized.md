---
title: HelpCustomized
description: HelpCustomized
MSHAttr:
- 'PreferredSiteName:MSDN'
- 'PreferredLib:/library/windows/hardware'
ms.assetid: 4494d414-b276-4bee-9c98-b358f9e26df2
ms.prod: W10
ms.mktglfcycl: deploy
ms.sitesec: msdn
---

# HelpCustomized


`HelpCustomized` specifies whether the Original Equipment Manufacturer (OEM) customizes Help. The outcome depends on the operating system:

-   In Windows 8, when you set this value to `true` and set values in Microsoft-Windows-HelpAndSupport\\[HelpAndSupport](helpandsupport-win8-microsoft-windows-helpandsupporthelpandsupport.md), you customize the **Windows Help and Support** page.

    For information about how to add customized Help files, see [Author and Add Custom Help and Support Content](http://go.microsoft.com/fwlink/?LinkId=237145).

-   In Windows 7 and Windows Vista, when you set this value to **true**, Control Panel shows a link to customized Help. Otherwise, it shows the support information that [SupportHours](supporthours-win7-microsoft-windows-shell-setupoeminformationsupporthours.md), [SupportPhone](supportphone-win7-microsoft-windows-shell-setupoeminformationsupportphone.md), and [SupportURL](supporturl-win7-microsoft-windows-shell-setupoeminformationsupporturl.md) specify.

    All information (including [Manufacturer](manufacturer-win7-microsoft-windows-shell-setupoeminformationmanufacturer.md) and [Model](model-win7-microsoft-windows-shell-setupoeminformationmodel.md)) should be in the customized Help file. This information doesn't appear in the **System** item in Control Panel.

## Values


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><strong>true</strong></p></td>
<td><p>Specifies that Help is customized.</p></td>
</tr>
<tr class="even">
<td><p><strong>false</strong></p></td>
<td><p>Specifies that Help isn't customized. This is the default value.</p></td>
</tr>
</tbody>
</table>

 

## Valid Configuration Passes


auditUser

generalize

offlineServicing

oobeSystem

specialize

## Parent Hierarchy


[Microsoft-Windows-Shell-Setup](microsoft-windows-shell-setup-win7-microsoft-windows-shell-setup.md) | [OEMInformation](oeminformation-win7-microsoft-windows-shell-setupoeminformation.md) | **HelpCustomized**

## Applies To


For a list of the Windows editions and architectures that this component supports, see [Microsoft-Windows-Shell-Setup](microsoft-windows-shell-setup-win7-microsoft-windows-shell-setup.md).

## XML Example


This XML shows how to specify that Help is customized:

``` syntax
<OEMInformation>
   <HelpCustomized>true</HelpCustomized>
   <Manufacturer><OEM name></Manufacturer>
   <Model><model name></Model>
   <Logo>C:\Windows\OEM\Logo.bmp</Logo>
   <SupportHours><hours></SupportHours>
   <SupportPhone>425-555-0190</SupportPhone>
   <SupportURL>http://www.contoso.com</SupportURL>
</OEMInformation>
```

## Related topics


[OEMInformation](oeminformation-win7-microsoft-windows-shell-setupoeminformation.md)

[HelpAndSupport](helpandsupport-win8-microsoft-windows-helpandsupporthelpandsupport.md)

[Author and Add Custom Help and Support Content](http://go.microsoft.com/fwlink/?LinkId=237145)

 

 

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20%5Bp_unattend\p_unattend%5D:%20HelpCustomized%20%20RELEASE:%20%2810/3/2016%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/default.aspx. "Send comments about this topic to Microsoft")





