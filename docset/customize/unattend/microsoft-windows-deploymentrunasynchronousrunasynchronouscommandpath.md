---
title: Path
description: Path
MSHAttr:
- 'PreferredSiteName:MSDN'
- 'PreferredLib:/library/windows/hardware'
ms.assetid: 3aa12be4-75f9-49a5-8d60-2f25d0f7be33
ms.prod: W10
ms.mktglfcycl: deploy
ms.sitesec: msdn
---

# Path


`Path` specifies the path and the name of the command to execute. [RunAsynchronous](microsoft-windows-deploymentrunasynchronous.md) commands run in the user context in the auditUser configuration pass and in the system context in the specialize configuration pass.

## Values


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><em>Path</em></p></td>
<td><p>Specifies the path and the file name of the command to execute asynchronously. The path can be a local path or a Universal Naming Convention (UNC) path. If the path is a UNC path, the [Credentials](microsoft-windows-deploymentrunasynchronousrunasynchronouscommandcredentials.md) setting must be specified.</p>
<p><em>Path</em> is a string with a maximum length of 259 characters.</p></td>
</tr>
</tbody>
</table>

 

This string type does not support empty elements. Do not create an empty value for this setting.

## Valid Passes


auditUser

specialize

## Parent Hierarchy


[Microsoft-Windows-Deployment](microsoft-windows-deployment.md) | [RunAsynchronous](microsoft-windows-deploymentrunasynchronous.md) | [RunAsynchronousCommand](microsoft-windows-deploymentrunasynchronousrunasynchronouscommand.md) | **Path**

## Applies To


For a list of the supported Windows® editions and architectures this component supports, see [Microsoft-Windows-Deployment](microsoft-windows-deployment-win7-microsoft-windows-deployment.md).

## XML Example


The following XML output shows how to set asynchronous commands.

The first command runs an application on the local hard drive. The command includes the environment variable %ProgramFiles%. The second command runs a command from the network.

``` syntax
<RunAsynchronous>
   <RunAsynchronousCommand wcm:action="add">
      <Description>AsynchCommand1</Description>
      <Order>1</Order>
      <Path>%ProgramFiles%\FabriKam\FabriKam First Run Application.exe</Path>
   </RunAsynchronousCommand>
   <RunAsynchronousCommand wcm:action="add">
      <Credentials>
         <Domain>MyDomain</Domain>
         <Password>MyPassword</Password>
         <Username>MyUsername</Username>
      </Credentials>
      <Description>SynchCommand2-FromNetwork</Description>
      <Order>2</Order>
      <Path>\\network\server\share\filename</Path>
   </RunAsynchronousCommand>
</RunAsynchronous>
```

## Related topics


[RunAsynchronousCommand](microsoft-windows-deploymentrunasynchronousrunasynchronouscommand.md)

 

 

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20%5Bp_unattend\p_unattend%5D:%20Path%20%20RELEASE:%20%2810/3/2016%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/default.aspx. "Send comments about this topic to Microsoft")





