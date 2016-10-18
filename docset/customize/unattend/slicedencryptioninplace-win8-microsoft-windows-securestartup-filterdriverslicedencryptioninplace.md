---
title: SlicedEncryptionInPlace
description: SlicedEncryptionInPlace
MSHAttr:
- 'PreferredSiteName:MSDN'
- 'PreferredLib:/library/windows/hardware'
ms.assetid: 7d4b2204-0147-49dd-b260-55766551ff65
ms.prod: W10
ms.mktglfcycl: deploy
ms.sitesec: msdn
---

# SlicedEncryptionInPlace


The `SlicedEncryptionInPlace` setting works with other settings in the [Microsoft-Windows-SecureStartup-FilterDriver](microsoft-windows-securestartup-filterdriver-win8-microsoft-windows-securestartup-filterdriver.md) component to optimize BitLocker settings for PCs with hardware architectures such as System on a Chip (SoC). Do not use these settings for standard 32-bit or 64-bit hardware architectures.

These settings are intended for OEM manufacturing only. For specific guidance on using these settings, contact Microsoft.

**Note**  
These settings only apply to Windows 8.

 

## Values


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><strong>0</strong></p></td>
<td><p>Slice requests are performed from a source to a target buffer.</p></td>
</tr>
<tr class="even">
<td><p><strong>1</strong></p></td>
<td><p>Slice requests are performed in place.</p>
<p>This is the default value.</p></td>
</tr>
</tbody>
</table>

 

## Valid Configuration Passes


offlineServicing

specialize

auditSystem

oobeSystem

## Parent Hierarchy


[Microsoft-Windows-SecureStartup-FilterDriver](microsoft-windows-securestartup-filterdriver-win8-microsoft-windows-securestartup-filterdriver.md) | **SlicedEncryptionInPlace**

## Applies To


For a list of the Windows editions and architectures that this component supports, see [Microsoft-Windows-SecureStartup-FilterDriver](microsoft-windows-securestartup-filterdriver-win8-microsoft-windows-securestartup-filterdriver.md).

## XML Example


The following example specifies recommended values for Bitlocker optimizations on an x86 System on a Chip.

``` syntax
<component name="Microsoft-Windows-SecureStartup-FilterDriver" processorArchitecture="x86" publicKeyToken="31bf3856ad364e35" language="neutral" versionScope="nonSxS" xmlns:wcm="http://schemas.microsoft.com/WMIConfig/2002/State" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
  <BytesDecryptedInDiskRequestOverhead>262144</BytesDecryptedInDiskRequestOverhead>
  <InPlaceCrypto>0</InPlaceCrypto>
  <MaxCryptoRequestsPerIo>4</MaxCryptoRequestsPerIo>
  <MaxDecryptRequests>0</MaxDecryptRequests>
  <MaxEncryptRequests>2</MaxEncryptRequests>
  <ModifiedWriteMaximum>4</ModifiedWriteMaximum>
  <ReadDoubleBuffering>0</ReadDoubleBuffering>
  <SlicedEncryptionInPlace>1</SlicedEncryptionInPlace>
  <SlicedEncryptionMinSize>524288</SlicedEncryptionMinSize>
  <SlicedEncryptionRequestsMax>1</SlicedEncryptionRequestsMax>
  <WriteIoAggregateMaxSize>1048576</WriteIoAggregateMaxSize>
  <WriteIoAggregateMinSize>1048576</WriteIoAggregateMinSize>
  <WriteSubrequestLength>524288</WriteSubrequestLength>
 </component>
```

## Related topics


[Microsoft-Windows-SecureStartup-FilterDriver](microsoft-windows-securestartup-filterdriver-win8-microsoft-windows-securestartup-filterdriver.md)

 

 

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20%5Bp_unattend\p_unattend%5D:%20SlicedEncryptionInPlace%20%20RELEASE:%20%2810/3/2016%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/default.aspx. "Send comments about this topic to Microsoft")





