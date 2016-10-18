---
title: RunAsynchronousCommand
description: RunAsynchronousCommand
MSHAttr:
- 'PreferredSiteName:MSDN'
- 'PreferredLib:/library/windows/hardware'
ms.assetid: cef754b4-9101-4d74-a036-66c4ed395f83
ms.prod: W10
ms.mktglfcycl: deploy
ms.sitesec: msdn
---

# RunAsynchronousCommand


`RunAsynchronousCommand` specifies a single command to run during the auditUser Configuration Pass or specialize Configuration Pass.

To run services or commands that can start at the same time, use asynchronous commands. To run commands that need to finish before other commands can start, use [RunSynchronousCommand](runsynchronouscommand-win7-microsoft-windows-deploymentrunsynchronousrunsynchronouscommand.md) instead.

`RunAsynchronous` commands run in the user context in the auditUser Configuration Pass and in the system context in the specialize Configuration Pass.

## Child Elements


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p>[Credentials](credentials-win7-microsoft-windows-deploymentrunasynchronousrunasynchronouscommandcredentials.md)</p></td>
<td><p>Specifies the credentials to use when accessing paths.</p></td>
</tr>
<tr class="even">
<td><p>[Description](description-win7-microsoft-windows-deploymentrunasynchronousrunasynchronouscommanddescription.md)</p></td>
<td><p>Specifies a description of the command to execute.</p></td>
</tr>
<tr class="odd">
<td><p>[Order](order-win7-microsoft-windows-deploymentrunasynchronousrunasynchronouscommandorder.md)</p></td>
<td><p>Specifies a unique value for each command.</p>
<div class="alert">
<strong>Important</strong>  
<p>The computer does not wait for one command to finish before it starts the next one.</p>
</div>
<div>
 
</div></td>
</tr>
<tr class="even">
<td><p>[Path](path-win7-microsoft-windows-deploymentrunasynchronousrunasynchronouscommandpath.md)</p></td>
<td><p>Specifies the path to the command to execute.</p></td>
</tr>
</tbody>
</table>

 

## Valid Configuration Passes


auditUser

specialize

## Parent Hierarchy


[Microsoft-Windows-Deployment](microsoft-windows-deployment-win7-microsoft-windows-deployment.md) | [RunAsynchronous](runasynchronous-win7-microsoft-windows-deploymentrunasynchronous.md) | **RunAsynchronousCommand**

## Applies To


For the list of the supported Windows editions and architectures this component supports, see [Microsoft-Windows-Deployment](microsoft-windows-deployment-win7-microsoft-windows-deployment.md).

## XML Example


The following XML output shows how to set asynchronous commands.

``` syntax
<RunAsynchronous>
   <RunAsynchronousCommand wcm:action="add">
      <Credentials>
         <Domain>MyDomain</Domain>
         <Password>MyPassword</Password>
         <Username>MyUsername</Username>
      </Credentials>
      <Description>AsynchCommand1</Description>
      <Order>1</Order>
      <Path>\\network\server\share\filename</Path>
   </RunAsynchronousCommand>
   <RunAsynchronousCommand wcm:action="add">
      <Credentials>
         <Domain>MyDomain</Domain>
         <Password>MyPassword</Password>
         <Username>MyUsername</Username>
      </Credentials>
      <Description>AsynchCommand2</Description>
      <Order>2</Order>
      <Path>\\network\server\share\filename</Path>
   </RunAsynchronousCommand>
</RunAsynchronous>
```

## Related topics


[RunAsynchronous](runasynchronous-win7-microsoft-windows-deploymentrunasynchronous.md)

[RunSynchronousCommand](runsynchronouscommand-win7-microsoft-windows-deploymentrunsynchronousrunsynchronouscommand.md)

 

 

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20%5Bp_unattend\p_unattend%5D:%20RunAsynchronousCommand%20%20RELEASE:%20%2810/3/2016%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/default.aspx. "Send comments about this topic to Microsoft")





