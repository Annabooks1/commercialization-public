---
title: Title
description: Title
MSHAttr:
- 'PreferredSiteName:MSDN'
- 'PreferredLib:/library/windows/hardware'
ms.assetid: 3073c3eb-b563-4887-b92e-d452669f434b
ms.prod: W10
ms.mktglfcycl: deploy
ms.sitesec: msdn
---

# Title


The `Title` setting specifies customized text to display next to the **Online Support** icon in the **Additional Information** page in the **Troubleshooting** Control Panel.

## Values


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><em>Title_ID</em></p></td>
<td><p>Specifies the title of the <strong>Online Support</strong> icon.</p>
<p><em>TitleID</em> is represented as <em>@dllname,-resourceID</em>, where <em>dllname</em> must include a full path to the resource DLL.</p>
<p>For information about creating localized versions of a DLL for each setting, see the MSDN topic: [Using the MUI with Applications](http://go.microsoft.com/fwlink/?LinkId=140252).</p></td>
</tr>
</tbody>
</table>

 

## Valid Configuration Passes


offlineServicing

generalize

specialize

## Parent Hierarchy


[Microsoft-Windows-DiagCpl](microsoft-windows-diagcpl-win7-microsoft-windows-diagcpl.md) | **Title**

## Applies To


For a list of the supported Windows® editions and architectures that this component supports, see [Microsoft-Windows-DiagCpl](microsoft-windows-diagcpl-win7-microsoft-windows-diagcpl.md).

## XML Example


The following XML output shows how to configure the **Online Support** icon to point to the Fabrikam Troubleshooting application.

``` syntax
  <Title>@%SystemRoot%\System32\DiagCpl.dll,-82</Title>
  <Description>@%SystemRoot%\System32\DiagCpl.dll,-83</Description>
  <Icon>@%SystemRoot%\System32\imageres.dll,-179</Icon>
  <Link>http://www.fabrikam.com/support</Link>
```

## Related topics


[Microsoft-Windows-DiagCpl](microsoft-windows-diagcpl-win7-microsoft-windows-diagcpl.md)

 

 

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20%5Bp_unattend\p_unattend%5D:%20Title%20%20RELEASE:%20%2810/3/2016%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/default.aspx. "Send comments about this topic to Microsoft")





