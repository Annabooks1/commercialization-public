---
title: microsoft-windows-international-core-winpe--
description: microsoft-windows-international-core-winpe--
MSHAttr:
- 'PreferredSiteName:MSDN'
- 'PreferredLib:/library/windows/hardware'
ms.assetid: 66c0e00c-12fe-4f2d-9be4-0b4a81634602
ms.mktglfcycl: deploy
ms.sitesec: msdn
ms.author: alhopper
ms.date: 05/02/2017
ms.topic: article
ms.prod: windows-hardware
ms.technology: windows-oem
---

# microsoft-windows-international-core-winpe--


The microsoft-windows-international-core-winpe-- component specifies the default language, locale, and other international settings to use during Windows Setup or Windows Deployment Services installations.

The settings in this component can be applied only in the windowsPE configuration pass. To specify language and locale settings in the oobeSystem and specialize configuration passes, see [Microsoft-Windows-International-Core](microsoft-windows-international-core.md).

## In This Section


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p>[InputLocale](microsoft-windows-international-core-winpe-inputlocale.md)</p></td>
<td><p>Specifies the system input locale and the keyboard layout.</p></td>
</tr>
<tr class="even">
<td><p>[LayeredDriver](microsoft-windows-international-core-winpe-layereddriver.md)</p></td>
<td><p>Specifies the keyboard driver to use for Japanese or Korean keyboards.</p></td>
</tr>
<tr class="odd">
<td><p>[SetupUILanguage](microsoft-windows-international-core-winpe-setupuilanguage.md)</p></td>
<td><p>Specifies the default language to use during Windows Setup or Windows Deployment Services.</p></td>
</tr>
<tr class="even">
<td><p>[SystemLocale](microsoft-windows-international-core-winpe-systemlocale.md)</p></td>
<td><p>Specifies the default language for non-Unicode programs.</p></td>
</tr>
<tr class="odd">
<td><p>[UILanguage](microsoft-windows-international-core-winpe-uilanguage.md)</p></td>
<td><p>Specifies the default system user interface (UI) language.</p></td>
</tr>
<tr class="even">
<td><p>[UILanguageFallback](microsoft-windows-international-core-winpe-uilanguagefallback.md)</p></td>
<td><p>Specifies the fallback language if the system default UI language is only partially localized.</p></td>
</tr>
<tr class="odd">
<td><p>[UserLocale](microsoft-windows-international-core-winpe-userlocale.md)</p></td>
<td><p>Specifies the per-user settings used for formatting dates, times, currency, and numbers.</p></td>
</tr>
</tbody>
</table>

 

## Applies To


To determine whether a component applies to the image you’re building, load your image into Windows SIM and search for the component or setting name. For information on how to view components and settings, see [Configure Components and Settings in an Answer File](https://docs.microsoft.com/en-us/windows-hardware/customize/desktop/wsim/configure-components-and-settings-in-an-answer-file).

## Related topics


[Components](components-b-unattend.md)

[Microsoft-Windows-International-Core](microsoft-windows-international-core.md)

 

 







