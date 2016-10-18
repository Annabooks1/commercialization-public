---
title: Order
description: Order
MSHAttr:
- 'PreferredSiteName:MSDN'
- 'PreferredLib:/library/windows/hardware'
ms.assetid: 25a1f7bc-2712-4ab4-9db2-08ca40ab7f85
ms.prod: W10
ms.mktglfcycl: deploy
ms.sitesec: msdn
---

# Order


`Order` specifies the order in which the [RunSynchronous](runsynchronous-win7-microsoft-windows-setuprunsynchronous.md) command is run.

Synchronous commands start in the order specified in the unattended installation answer file, and each command must finish before the next command starts.

To start a command that needs to finish before other commands can start, use synchronous commands. To run services or commands that can start at the same time, use [RunAsynchronous](runasynchronous-win7-microsoft-windows-setuprunasynchronous.md) instead.

All [RunSynchronous](runsynchronous-win7-microsoft-windows-setuprunsynchronous.md) commands run in the system context.

## Values


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><em>Synchronous_command_execution_order</em></p></td>
<td><p>Specifies the order to start the command. This value is an integer between 1 and 500.</p></td>
</tr>
</tbody>
</table>

 

## Valid Configuration Passes


windowsPE

## Parent Hierarchy


[Microsoft-Windows-Setup](microsoft-windows-setup-win7-microsoft-windows-setup.md) | [RunSynchronous](runsynchronous-win7-microsoft-windows-setuprunsynchronous.md) | [RunSynchronousCommand](runsynchronouscommand-win7-microsoft-windows-setuprunsynchronousrunsynchronouscommand.md) | **Order**

## Applies To


For a list of the supported Windows® editions and architectures that this component supports, see [Microsoft-Windows-Setup](microsoft-windows-setup-win7-microsoft-windows-setup.md).

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


[RunSynchronousCommand](runsynchronouscommand-win7-microsoft-windows-setuprunsynchronousrunsynchronouscommand.md)

[RunAsynchronous](runasynchronous-win7-microsoft-windows-setuprunasynchronous.md)

 

 

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20%5Bp_unattend\p_unattend%5D:%20Order%20%20RELEASE:%20%2810/3/2016%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/default.aspx. "Send comments about this topic to Microsoft")





