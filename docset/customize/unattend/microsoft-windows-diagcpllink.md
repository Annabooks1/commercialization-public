---
title: Link
description: Link
MSHAttr:
- 'PreferredSiteName:MSDN'
- 'PreferredLib:/library/windows/hardware'
ms.assetid: 8d5c2f06-d09f-4e14-8a6c-2a5bfe10e888
ms.prod: W10
ms.mktglfcycl: deploy
ms.sitesec: msdn
---

# Link


The `Link` setting specifies a GUID of the **Online Support** icon in the **Additional Information** page located in the **Troubleshooting** Control Panel.

For information about finding the GUID for your icon, see the MSDN topic: [NOTIFYICONDATA Structure](http://go.microsoft.com/fwlink/?LinkId=120340).

## Values


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><em>GUID</em> or <em>URL</em></p></td>
<td><p>Specifies either a <em>GUID</em> of an application or a <em>URL</em> to a website which is called when the user selects the <strong>Online Support</strong> icon.</p></td>
</tr>
</tbody>
</table>

 

## Valid Configuration Passes


offlineServicing

generalize

specialize

## Parent Hierarchy


[Microsoft-Windows-DiagCpl](microsoft-windows-diagcpl-win7-microsoft-windows-diagcpl.md) | **Link**

## Applies To


For a list of the supported Windows® editions and architectures that this component supports, see [Microsoft-Windows-DiagCpl](microsoft-windows-diagcpl-win7-microsoft-windows-diagcpl.md).

## XML Example


The following XML output shows how to configure the **Additional Information** icon to point to the Fabrikam Troubleshooting application by using a GUID to specify the application location.

``` syntax
  <Title>@%SystemRoot%\System32\DiagCpl.dll,-82</Title>
  <Description>@%SystemRoot%\System32\DiagCpl.dll,-83</Description>
  <Icon>@%SystemRoot%\System32\imageres.dll,-179</Icon>
  <Link>{abcde-01234-fabc01234def-39393}</Link>
```

The following XML output shows how to configure the **Additional Information** icon to point to the Fabrikam Support website by using a URL.

``` syntax
  <Title>@%SystemRoot%\System32\DiagCpl.dll,-82</Title>
  <Description>@%SystemRoot%\System32\DiagCpl.dll,-83</Description>
  <Icon>@%SystemRoot%\System32\imageres.dll,-179</Icon>
  <Link>http://www.fabrikam.com/support</Link>
```

## Related topics


[Microsoft-Windows-DiagCpl](microsoft-windows-diagcpl-win7-microsoft-windows-diagcpl.md)

 

 

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20%5Bp_unattend\p_unattend%5D:%20Link%20%20RELEASE:%20%2810/3/2016%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/default.aspx. "Send comments about this topic to Microsoft")





