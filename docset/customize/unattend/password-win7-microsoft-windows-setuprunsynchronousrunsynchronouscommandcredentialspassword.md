---
title: Password
description: Password
MSHAttr:
- 'PreferredSiteName:MSDN'
- 'PreferredLib:/library/windows/hardware'
ms.assetid: a95eb9d9-3a5b-4320-8fe2-879a01ee41d2
ms.prod: W10
ms.mktglfcycl: deploy
ms.sitesec: msdn
---

# Password


`Password` specifies the password of the user account used to authentication access to the location specified by [Path](path-win7-microsoft-windows-setuprunsynchronousrunsynchronouscommandpath.md).

All [RunSynchronous](runsynchronous-win7-microsoft-windows-setuprunsynchronous.md) commands run in the system context.

## Values


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><em>Password</em></p></td>
<td><p>Specifies the password of the user account used for authentication. <em>Password</em> is a string.</p></td>
</tr>
</tbody>
</table>

 

This string type does not support empty elements. Do not create an empty value for this setting.

## Valid Passes


windowsPE

## Parent Hierarchy


[Microsoft-Windows-Setup](microsoft-windows-setup-win7-microsoft-windows-setup.md) | [RunSynchronous](runsynchronous-win7-microsoft-windows-setuprunsynchronous.md) | [RunSynchronousCommand](runsynchronouscommand-win7-microsoft-windows-setuprunsynchronousrunsynchronouscommand.md) | [Credentials](credentials-win7-microsoft-windows-setuprunsynchronousrunsynchronouscommandcredentials.md) | **Pasword**

## Applies To


For the list of the supported Windows editions and architectures that this component supports, see [Microsoft-Windows-Setup](microsoft-windows-setup-win7-microsoft-windows-setup.md).

## XML Example


The following XML output shows how to set synchronous commands.

``` syntax
<RunSynchronous>
   <!-- First synchronous command to execute -->
   <RunSynchronousCommand>
      <Order>1</Order>
      <Path>\\MyNetworkShare\MyApplication.exe</Path>
      <Description>DescriptionOfMyApplication</Description>
      <Credentials>
         <Domain>FabrikamDomain</Domain>
         <UserName>MyUserName</UserName>
         <Password>MyPassword</Password>
      </Credentials>
   </RunSynchronousCommand>
<!-- Second synchronous command to execute -->
   <RunSynchronousCommand>
      <Order>2</Order>
      <Path>C:\AnotherApplication.exe</Path>
      <Description>DescriptionOfMyApplication</Description>
   </RunSynchronousCommand>
</RunSynchronous>
```

## Related topics


[Credentials](credentials-win7-microsoft-windows-setuprunsynchronousrunsynchronouscommandcredentials.md)

 

 

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20%5Bp_unattend\p_unattend%5D:%20Password%20%20RELEASE:%20%2810/3/2016%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/default.aspx. "Send comments about this topic to Microsoft")





