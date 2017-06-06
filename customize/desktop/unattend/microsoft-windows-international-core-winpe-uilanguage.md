---
title: UILanguage
description: UILanguage
MSHAttr:
- 'PreferredSiteName:MSDN'
- 'PreferredLib:/library/windows/hardware'
ms.assetid: 23da0462-281c-4f2b-a55d-3a395c86b433
ms.prod: W10
ms.mktglfcycl: deploy
ms.sitesec: msdn
ms.author: alhopper
ms.date: 05/02/2017
ms.topic: article
ms.prod: windows-hardware
ms.technology: windows-oem
---

# UILanguage


`UILanguage` specifies the language that will be used as the default system language to display user interface (UI) items (such as menus, dialog boxes, and Help files).

This setting is used by Windows Setup and Windows Deployment Services.

For a list of supported languages, see [Supported Language Packs and Default Settings](http://go.microsoft.com/fwlink/p/?linkid=200317).

In upgrade installation types, this setting is ignored. In upgrade installations, you can upgrade only from the same language.

## Values


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><em>UI_language</em></p></td>
<td><p>Specifies the language of the UI.</p>
<p>The <em>UI_language</em> string is based on the language-tagging conventions of RFC 3066. The pattern <em>language-region</em> is used, where <em>language</em> is a language code and <em>region</em> is a country or region identifier (for example, <strong>en-US</strong>, <strong>fr-FR</strong>, or <strong>es-ES</strong>).</p>
<p>This value is not case-sensitive.</p></td>
</tr>
</tbody>
</table>

 

This string type supports empty elements.

## Parent Hierarchy


[microsoft-windows-international-core-winpe--](microsoft-windows-international-core-winpe.md) | **UILanguage**

## Valid Configuration Passes


windowsPE

## Applies To


For the list of the Windows editions and architectures that this component supports, see [microsoft-windows-international-core-winpe--](microsoft-windows-international-core-winpe.md).

## XML Example


The following example shows how to set the UI language to German (Germany).

``` syntax
<InputLocale>0407:00000407</InputLocale> 
<SystemLocale>de-DE</SystemLocale> 
<UILanguage>de-DE</UILanguage> 
<UserLocale>de-DE</UserLocale>
```

## Related topics


[Microsoft-Windows-International-Core](microsoft-windows-international-core.md)

 

 

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20%5Bp_unattend\p_unattend%5D:%20UILanguage%20%20RELEASE:%20%2810/3/2016%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/default.aspx. "Send comments about this topic to Microsoft")





