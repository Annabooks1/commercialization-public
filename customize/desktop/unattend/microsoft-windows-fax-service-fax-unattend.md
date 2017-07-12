---
title: FaxUnattend
description: FaxUnattend
MSHAttr:
- 'PreferredSiteName:MSDN'
- 'PreferredLib:/library/windows/hardware'
ms.assetid: f4ae8d99-6d03-4373-abad-2bfec81f4b4e
ms.mktglfcycl: deploy
ms.sitesec: msdn
ms.author: alhopper
ms.date: 05/02/2017
ms.topic: article
ms.prod: windows-hardware
ms.technology: windows-oem
---

# FaxUnattend


`FaxUnattend` specifies details about sending, receiving, printing, and saving faxes.

## Child Elements


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p>[Csid](microsoft-windows-fax-service-fax-unattend-csid.md)</p></td>
<td><p>Specifies the called subscriber ID (CSID) transmitted to the sending fax machine when receiving incoming faxes.</p></td>
</tr>
<tr class="even">
<td><p>[FaxPrinterIsShared](microsoft-windows-fax-service-fax-unattend-faxprinterisshared.md)</p></td>
<td><p>Specifies if the fax printer is shared and if remote users can use the server as a shared fax server.</p></td>
</tr>
<tr class="odd">
<td><p>[ReceiveFaxes](microsoft-windows-fax-service-fax-unattend-receivefaxes.md)</p></td>
<td><p>Specifies whether the fax service answers incoming calls on a device. This entry applies to existing and new fax devices.</p></td>
</tr>
<tr class="even">
<td><p>[Rings](microsoft-windows-fax-service-fax-unattend-rings.md)</p></td>
<td><p>Specifies the number of rings before the fax service answers the telephone. This entry applies to existing and new fax devices.</p></td>
</tr>
<tr class="odd">
<td><p>[RouteFolderName](microsoft-windows-fax-service-fax-unattend-routefoldername.md)</p></td>
<td><p>Specifies the folder name to which the fax service automatically routes and saves incoming faxes.</p></td>
</tr>
<tr class="even">
<td><p>[RoutePrinterName](microsoft-windows-fax-service-fax-unattend-routeprintername.md)</p></td>
<td><p>Specifies the printer name to which the fax service routes (prints) incoming faxes automatically.</p></td>
</tr>
<tr class="odd">
<td><p>[RouteToFolder](microsoft-windows-fax-service-fax-unattend-routetofolder.md)</p></td>
<td><p>Specifies whether to route incoming faxes to a folder.</p></td>
</tr>
<tr class="even">
<td><p>[RouteToPrinter](microsoft-windows-fax-service-fax-unattend-routetoprinter.md)</p></td>
<td><p>Specifies whether to route incoming faxes to a printer.</p></td>
</tr>
<tr class="odd">
<td><p>[SendFaxes](microsoft-windows-fax-service-fax-unattend-sendfaxes.md)</p></td>
<td><p>Specifies whether the fax service uses a device to send faxes. This entry applies to existing and new fax devices.</p></td>
</tr>
<tr class="even">
<td><p>[Tsid](microsoft-windows-fax-service-fax-unattend-tsid.md)</p></td>
<td><p>Specifies the transmitting subscriber ID (TSID) sent by the fax device to a receiving fax machine.</p></td>
</tr>
</tbody>
</table>

 

## Valid Passes


specialize

## Parent Hierarchy


[Microsoft-Windows-Fax-Service](microsoft-windows-fax-service.md) | **FaxUnattend**

## Applies To


For a list of the supported Windows editions and architectures that this component supports, see [Microsoft-Windows-Fax-Service](microsoft-windows-fax-service.md).

## XML Example


The following XML output shows how to set fax settings.

``` syntax
<Fax>
   <ArchiveFaxes>false</ArchiveFaxes>
   <IncomingFaxesArePublic>false</IncomingFaxesArePublic>
   <ArchiveFolderName>C:\MyFaxArchives</ArchiveFolderName>
</Fax>
<FaxUnattend>
   <FaxPrinterIsShared>true</FaxPrinterIsShared>
   <ReceiveFaxes>false</ReceiveFaxes>
   <Rings>6</Rings>
   <RouteToFolder>true</RouteToFolder>
   <RouteToPrinter>true</RouteToPrinter>
   <SendFaxes>true</SendFaxes>
   <Csid>Fax1</Csid>
   <Tsid>Fax1</Tsid>
   <RouteFolderName>C:\Router</RouteFolderName>
   <RoutePrinterName>C:\Printer</RoutePrinterName>
</FaxUnattend>
<Receipts>
   <FaxUserName>MyUserName</FaxUserName>
   <FaxUserPassword>MyPassword</FaxUserPassword>
   <SmtpNotificationsEnabled>true</SmtpNotificationsEnabled>
   <SmtpSenderAddress>MyUserName@fabrikam.com</SmtpSenderAddress>
   <SmtpServerAddress>207.46.197.32</SmtpServerAddress>
   <SmtpServerAuthenticationMechanism>1</SmtpServerAuthenticationMechanism>
   <SmtpServerPort>26</SmtpServerPort>
</Receipts>
```

## Related topics


[Microsoft-Windows-Fax-Service](microsoft-windows-fax-service.md)

 

 







