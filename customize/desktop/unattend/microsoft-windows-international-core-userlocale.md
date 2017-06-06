---
title: UserLocale
description: UserLocale
MSHAttr:
- 'PreferredSiteName:MSDN'
- 'PreferredLib:/library/windows/hardware'
ms.assetid: 31880e1a-2f40-4d8b-b6f0-c1799911ed39
ms.prod: W10
ms.mktglfcycl: deploy
ms.sitesec: msdn
ms.author: alhopper
ms.date: 05/02/2017
ms.topic: article
ms.prod: windows-hardware
ms.technology: windows-oem
---

# UserLocale


`UserLocale` specifies the per-user settings used for formatting dates, times, currency, and numbers in a Windows installation.

Users can change this value on a running Windows installation by using the **Administrative** pane in the **Region and Language** Control Panel.

For a list of supported languages, locales, and identifiers, see [Available Language Packs](http://go.microsoft.com/fwlink/?LinkId=206620).

## Values


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><em>User_locale</em></p></td>
<td><p>Specifies the locale of the end user.</p>
<p>The <em>User_locale</em> string is based on the language-tagging conventions of RFC 3066. The pattern <em>language</em>-<em>region</em> is used, where <em>language</em> is a language code and <em>region</em> is a country or region identifier (for example, <strong>en-US</strong>, <strong>fr-FR</strong>, or <strong>es-ES</strong>).</p>
<p>This value is not case-sensitive.</p></td>
</tr>
</tbody>
</table>

 

This string type supports empty elements.

## Parent Hierarchy


[Microsoft-Windows-International-Core](microsoft-windows-international-core.md) | **UserLocale**

## Valid Configuration Passes


oobeSystem

specialize

## Applies To


For a list of the Windows editions and architectures that this component supports, see [Microsoft-Windows-International-Core](microsoft-windows-international-core.md).

## XML Example


The following example shows how to set the user locale to Japanese (Japan).

``` syntax
<InputLocale>0411:00000411</InputLocale> 
<SystemLocale>ja-JP</SystemLocale> 
<UILanguage>ja-JP</UILanguage> 
<UserLocale>ja-JP</UserLocale>
```

## Related topics


[Available Language Packs](http://go.microsoft.com/fwlink/p/?linkid=200318)

[Microsoft-Windows-International-Core](microsoft-windows-international-core.md)

 

 

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20%5Bp_unattend\p_unattend%5D:%20UserLocale%20%20RELEASE:%20%2810/3/2016%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/default.aspx. "Send comments about this topic to Microsoft")





