---
title: InstallFrom
description: InstallFrom
MSHAttr:
- 'PreferredSiteName:MSDN'
- 'PreferredLib:/library/windows/hardware'
ms.assetid: b448ca50-b973-4c8e-98aa-e354df58ba0a
ms.prod: W10
ms.mktglfcycl: deploy
ms.sitesec: msdn
---

# InstallFrom


`InstallFrom` specifies the Windows® image (.wim) file that contains the image to install and the credentials used to access the file.

## Child Elements


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p>[Credentials](credentials-win7-microsoft-windows-setupimageinstallosimageinstallfromcredentials.md)</p></td>
<td><p>Specifies the credentials used to access the .wim file.</p></td>
</tr>
<tr class="even">
<td><p>[MetaData](metadata-win7-microsoft-windows-setupimageinstallosimageinstallfrommetadata.md)</p></td>
<td><p>Specifies a unique Windows image in the .wim file to install.</p></td>
</tr>
<tr class="odd">
<td><p>[Path](path-win7-microsoft-windows-setupimageinstallosimageinstallfrompath.md)</p></td>
<td><p>Specifies the path to the .wim file.</p></td>
</tr>
</tbody>
</table>

 

## Valid Passes


windowsPE

## Parent Hierarchy


[Microsoft-Windows-Setup](microsoft-windows-setup-win7-microsoft-windows-setup.md) | [ImageInstall](imageinstall-win7-microsoft-windows-setupimageinstall.md) | [OSImage](osimage-win7-microsoft-windows-setupimageinstallosimage.md) | **InstallFrom**

## Applies To


For a list of the supported Windows editions and architectures that this component supports, see [Microsoft-Windows-Setup](microsoft-windows-setup-win7-microsoft-windows-setup.md).

## XML Example


The following XML output shows how to set the `ImageInstall` setting to install both an operating system image and a data image.

``` syntax
<ImageInstall>
    <OSImage>
        <InstallFrom>
            <Credentials>
                <Domain>FabrikamDomain</Domain>
                <Password>MyPassword</Password>
                <Username>MyUsername</Username>
            </Credentials>
            <Path>\\networkshare\share\install.wim</Path>
            <MetaData wcm:action="add">
                <Key>/IMAGE/NAME</Key>
                <Value>FabrikamCustomOSImage</Value>
            </MetaData>
        </InstallFrom>
        <InstallTo>
            <DiskID>0</DiskID>
            <PartitionID>1</PartitionID>
        </InstallTo>
        <WillShowUI>OnError</WillShowUI>
        <InstallToAvailablePartition>false</InstallToAvailablePartition>
    </OSImage>
    <DataImage wcm:action="add">
        <InstallTo>
            <DiskID>0</DiskID>
            <PartitionID>2</PartitionID>
        </InstallTo>
        <InstallFrom>
            <Credentials>
                <Domain>FabrikamDomain</Domain>
                <Password>MyPassword</Password>
                <Username>MyUsername</Username>
            </Credentials>
            <Path>\\networkshare\share\data.wim</Path>
            <MetaData wcm:action="add">
                <Key>/IMAGE/NAME</Key>
                <Value>FabrikamData</Value>
            </MetaData>
        </InstallFrom>
        <Order>1</Order>
    </DataImage>
</ImageInstall>
```

## Related topics


[OSImage](osimage-win7-microsoft-windows-setupimageinstallosimage.md)

 

 

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20%5Bp_unattend\p_unattend%5D:%20InstallFrom%20%20RELEASE:%20%2810/3/2016%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/default.aspx. "Send comments about this topic to Microsoft")





