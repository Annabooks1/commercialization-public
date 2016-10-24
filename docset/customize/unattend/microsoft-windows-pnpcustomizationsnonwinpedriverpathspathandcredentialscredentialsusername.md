---
title: Username
description: Username
MSHAttr:
- 'PreferredSiteName:MSDN'
- 'PreferredLib:/library/windows/hardware'
ms.assetid: 8d7f211e-52fc-41eb-84f6-811bed287421
ms.prod: W10
ms.mktglfcycl: deploy
ms.sitesec: msdn
---

# Username


`Username` specifies the name of the account to use for authentication.

## Values


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><em>User_name</em></p></td>
<td><p>Specifies the user name of the account used to authenticate the [Path](microsoft-windows-pnpcustomizationsnonwinpedriverpathspathandcredentialspath.md).</p>
<p><em>User_name</em> is a string.</p></td>
</tr>
</tbody>
</table>

 

This string type supports empty elements.

## Valid Passes


auditSystem

offlineServicing

## Parent Hierarchy


[Microsoft-Windows-PnpCustomizationsNonWinPE](microsoft-windows-pnpcustomizationsnonwinpe-win7-microsoft-windows-pnpcustomizationsnonwinpe.md) | [DriverPaths](microsoft-windows-pnpcustomizationsnonwinpedriverpaths.md) | [PathAndCredentials](microsoft-windows-pnpcustomizationsnonwinpedriverpathspathandcredentials.md) | [Credentials](microsoft-windows-pnpcustomizationsnonwinpedriverpathspathandcredentialscredentials.md) | **Username**

## Applies To


For the list of the supported Windows editions and architectures that this component supports, see [Microsoft-Windows-PnpCustomizationsNonWinPE](microsoft-windows-pnpcustomizationsnonwinpe-win7-microsoft-windows-pnpcustomizationsnonwinpe.md).

## XML Example


The following XML output specifies the Universal Naming Convention (UNC) paths to two additional locations for device drivers and the credentials used to access those paths.

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


[Credentials](microsoft-windows-pnpcustomizationsnonwinpedriverpathspathandcredentialscredentials.md)

 

 

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20%5Bp_unattend\p_unattend%5D:%20Username%20%20RELEASE:%20%2810/3/2016%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/default.aspx. "Send comments about this topic to Microsoft")





