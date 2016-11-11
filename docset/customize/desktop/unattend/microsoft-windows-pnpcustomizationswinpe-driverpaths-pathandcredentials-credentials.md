---
title: Credentials
description: Credentials
MSHAttr:
- 'PreferredSiteName:MSDN'
- 'PreferredLib:/library/windows/hardware'
ms.assetid: 1ecbaae7-0509-4f5d-918f-610332730109
ms.prod: W10
ms.mktglfcycl: deploy
ms.sitesec: msdn
---

# Credentials


`Credentials` is an optional setting used to access the Universal Naming Convention (UNC) path specified by the [Path](microsoft-windows-pnpcustomizationswinpe-driverpaths-pathandcredentials-path.md).

## Child Elements


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p>[Domain](microsoft-windows-pnpcustomizationswinpe-driverpaths-pathandcredentials-credentials-domain.md)</p></td>
<td><p>Specifies the domain of the account used for authentication. If the account is not a domain account, then the computer name should be used instead of the domain name.</p></td>
</tr>
<tr class="even">
<td><p>[Password](microsoft-windows-pnpcustomizationswinpe-driverpaths-pathandcredentials-credentials-password.md)</p></td>
<td><p>Specifies the password of the account used for authentication.</p></td>
</tr>
<tr class="odd">
<td><p>[Username](microsoft-windows-pnpcustomizationswinpe-driverpaths-pathandcredentials-credentials-username.md)</p></td>
<td><p>Specifies the user name of the account.</p></td>
</tr>
</tbody>
</table>

 

## Valid Passes


windowsPE

## Parent Hierarchy


[microsoft-windows-pnpcustomizationswinpe-](microsoft-windows-pnpcustomizationswinpe.md) | [DriverPaths](microsoft-windows-pnpcustomizationswinpe-driverpaths.md) | [PathAndCredentials](microsoft-windows-pnpcustomizationswinpe-driverpaths-pathandcredentials.md) | **Credentials**

## Applies To


For the list of the supported Windows editions and architectures that this component supports, see [microsoft-windows-pnpcustomizationswinpe-](microsoft-windows-pnpcustomizationswinpe--win7-microsoft-windows-pnpcustomizationswinpe.md).

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


[PathAndCredentials](microsoft-windows-pnpcustomizationswinpe-driverpaths-pathandcredentials.md)

 

 

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20%5Bp_unattend\p_unattend%5D:%20Credentials%20%20RELEASE:%20%2810/3/2016%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/default.aspx. "Send comments about this topic to Microsoft")





