---
title: DriverPaths
description: DriverPaths
MSHAttr:
- 'PreferredSiteName:MSDN'
- 'PreferredLib:/library/windows/hardware'
ms.assetid: 9fc40cc0-1858-4526-9cbb-f580eb080d86
ms.prod: W10
ms.mktglfcycl: deploy
ms.sitesec: msdn
---

# DriverPaths


`DriverPaths` specifies one or more paths that contain out-of-box drivers. These out-of-box drivers are copied to the Windows® image during the **windowsPE** configuration pass. `DriverPaths` is a container for one or more [PathAndCredentials](microsoft-windows-pnpcustomizationswinpedriverpathspathandcredentials.md) list items.

By using this setting, you can add boot-critical and non boot–critical drivers to your Windows image before it is installed.

## Child Elements


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p>[PathAndCredentials](microsoft-windows-pnpcustomizationswinpedriverpathspathandcredentials.md)</p></td>
<td><p>Specifies a local or Universal Naming Convention (UNC) path to the out-of-box drivers and, optionally, the [Credentials](microsoft-windows-pnpcustomizationswinpedriverpathspathandcredentialscredentials.md) used to access them.</p></td>
</tr>
</tbody>
</table>

 

## Valid Configuration Passes


windowsPE

## Parent Hierarchy


[Microsoft-Windows-PnpCustomizationsWinPE](microsoft-windows-pnpcustomizationswinpe-win7-microsoft-windows-pnpcustomizationswinpe.md) | **DriverPaths**

## Applies To


For a list of the supported Windows editions and architectures that this component supports, see [Microsoft-Windows-PnpCustomizationsWinPE](microsoft-windows-pnpcustomizationswinpe-win7-microsoft-windows-pnpcustomizationswinpe.md).

## XML Example


The following XML output specifies the UNC paths to additional locations for device drivers and the credentials used to access those paths.

``` syntax
<DriverPaths>
<!-- First PathAndCredentials list item -->
   <PathAndCredentials wcm:action="add" wcm:keyValue="1">
      <Path>\\myFirstDriverPath\DriversFolder</Path>
      <Credentials>
         <Domain>MyDomain</Domain>
         <Username>MyUsername</Username>
         <Password>MyPassword</Password>
      </Credentials>
   </PathAndCredentials>
<!-- Second PathAndCredentials list item -->
   <PathAndCredentials wcm:action="add" wcm:keyValue="2">
      <Path>C:\Drivers</Path>
      <Credentials>
         <Domain>MyComputerName</Domain>
         <Username>MyUsername</Username>
         <Password>MyPassword</Password>
      </Credentials>
   </PathAndCredentials>
</DriverPaths>
```

## Related topics


[Microsoft-Windows-PnpCustomizationsWinPE](microsoft-windows-pnpcustomizationswinpe-win7-microsoft-windows-pnpcustomizationswinpe.md)

 

 

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20%5Bp_unattend\p_unattend%5D:%20DriverPaths%20%20RELEASE:%20%2810/3/2016%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/default.aspx. "Send comments about this topic to Microsoft")





