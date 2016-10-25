---
title: JoinDomain
description: JoinDomain
MSHAttr:
- 'PreferredSiteName:MSDN'
- 'PreferredLib:/library/windows/hardware'
ms.assetid: 196de9ea-c3a4-4994-9e68-b3a1d90ff187
ms.prod: W10
ms.mktglfcycl: deploy
ms.sitesec: msdn
---

# JoinDomain


`JoinDomain` specifies the name of the domain to join. If this value is set, [JoinWorkgroup](microsoft-windows-unattendedjoinidentificationjoinworkgroup.md) cannot be set.

## Values


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><em>Domain_name</em></p></td>
<td><p>Specifies the name of the domain to join during Windows Setup. <em>Domain_name</em> can be the fully qualified Domain Name System (DNS) name of the domain or the NetBIOS name of the domain. <em>Domain_name</em> is a string.</p>
<p>You can specify either a domain to join or a workgroup to assign by using the <code>JoinDomain</code> or [JoinWorkgroup](microsoft-windows-unattendedjoinidentificationjoinworkgroup.md) settings respectively. However, only one of these settings should be present in an answer file. If both exist in an answer file, the value for <code>JoinDomain</code> is used, and JoinWorkgroup is ignored.</p></td>
</tr>
</tbody>
</table>

 

This string type does not support empty elements. Do not create an empty value for this setting.

## Valid Passes


specialize

## Parent Hierarchy


[Microsoft-Windows-UnattendedJoin](microsoft-windows-unattendedjoin.md) | [Identification](microsoft-windows-unattendedjoinidentification.md) | **JoinDomain**

## Applies To


For a list of the supported Windows® editions and architectures that this component supports, see [Microsoft-Windows-UnattendedJoin](microsoft-windows-unattendedjoin-win7-microsoft-windows-unattendedjoin.md).

## XML Example


The following XML output shows how to set the identification credentials.

``` syntax
<Identification>
   <Credentials>
      <Domain>fabrikam.com</Domain>
      <Password>MyPassword</Password>
      <Username>MyUserName</Username>
   </Credentials>
   <JoinDomain>fabrikam.com</JoinDomain>
   <MachinePassword>ComputerPassword</MachinePassword>
</Identification>
```

## Related topics


[Identification](microsoft-windows-unattendedjoinidentification.md)

 

 

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20%5Bp_unattend\p_unattend%5D:%20JoinDomain%20%20RELEASE:%20%2810/3/2016%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/default.aspx. "Send comments about this topic to Microsoft")





