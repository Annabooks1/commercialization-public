---
title: OemExtensionXmlFilePath
description: OemExtensionXmlFilePath
MSHAttr:
- 'PreferredSiteName:MSDN'
- 'PreferredLib:/library/windows/hardware'
ms.assetid: 4f507e62-de65-4937-80fc-3d20fb826788
ms.prod: W10
ms.mktglfcycl: deploy
ms.sitesec: msdn
---

# OemExtensionXmlFilePath


**Warning**  
This setting is deprecated. By default, the Initial Configurations Tasks application does not appear in Windows Server® 2012. Use [Microsoft-Windows-ServerManager-SvrMgrNc](microsoft-windows-servermanager-svrmgrnc-win7-microsoft-windows-servermanager-svrmgrnc.md) instead.

 

`OemExtensionXmlFilePath` specifies the path to the OEM XML file that contains the OEM resources and tasks that are displayed in the Initial Configuration Tasks and Server applications. OEMs are able to add information and links to Help topics and their own applications that need to be started.

The OEM XML file must be located in either the `%WINDIR%\system32` directory or in one of its subdirectories. For example, `C:\windows\system32\OEM\OEMExtension.xml`

## Values


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><em>File_path</em></p></td>
<td><p>Specifies the path to the OEM XML file that contains the OEM resources and tasks that are displayed in the Initial Configuration Tasks and Server applications. <em>File_path</em> is a string.</p></td>
</tr>
</tbody>
</table>

 

## Valid Configuration Passes


generalize

specialize

## Parent Hierarchy


[Microsoft-Windows-OutOfBoxExperience](mmicrosoft-windows-outofboxexperience.md) | **OemExtensionXmlFilePath**

## Applies To


For a list of the supported Windows® editions and architectures that this component supports, see [Microsoft-Windows-OutOfBoxExperience](microsoft-windows-outofboxexperience-win7-microsoft-windows-outofboxexperience.md).

## XML Example


The following XML output specifies the path to the OEM XML file that contains the OEM resources and tasks that are displayed in the Initial Configuration Tasks and Server applications.

``` syntax
<OemExtensionXmlFilePath>C:\windows\system32\OEM\OEMExtension.xml</OemExtensionXmlFilePath>
```

## Related topics


[Microsoft-Windows-OutOfBoxExperience](microsoft-windows-outofboxexperience.md)

 

 

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20%5Bp_unattend\p_unattend%5D:%20OemExtensionXmlFilePath%20%20RELEASE:%20%2810/3/2016%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/default.aspx. "Send comments about this topic to Microsoft")





