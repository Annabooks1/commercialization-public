---
title: Hide the auto brightness setting
description: OEMs can hide the automatic brightness setting for phones that do not have an ambient light sensor.
MSHAttr:
- 'PreferredSiteName:MSDN'
- 'PreferredLib:/library/windows/hardware'
ms.assetid: 81255b22-afcd-43e8-bf0c-8af3926900ac
ms.author: windows-hardware-design-content
ms.date: 05/02/2017
ms.topic: article
ms.prod: windows-hardware
ms.technology: windows-devices
---

# Hide the auto brightness setting


OEMs can hide the automatic brightness setting for phones that do not have an ambient light sensor.

<a href="" id="constraints---imagetimeonly"></a>**Constraints:** ImageTimeOnly  

<a href="" id="instructions-"></a>**Instructions:**  
1.  Create a customization answer file using the contents shown in the following code sample.

    ``` syntax
    <?xml version="1.0" encoding="utf-8" ?>  
    <ImageCustomizations xmlns="http://schemas.microsoft.com/embedded/2004/10/ImageUpdate"  
                         Name="HideAutoBrightness"  
                         Description="Use to hide the auto brightness setting for phones without an ambient light sensor."  
                         Owner=""  
                         OwnerType="OEM"> 
      
      <Static>  

        <Settings Path="Brightness">  
          <Setting Name="HideAutoBrightness" Value="" />
        </Settings>  

      </Static>

    </ImageCustomizations>
    ```

2.  Specify an `Owner`.

3.  Set `Value` to one of the following:

    <table>
    <colgroup>
    <col width="50%" />
    <col width="50%" />
    </colgroup>
    <thead>
    <tr class="header">
    <th>Value</th>
    <th>Description</th>
    </tr>
    </thead>
    <tbody>
    <tr class="odd">
    <td><p>0 or 'Show'</p></td>
    <td><p>Use to show the <strong>Automatically adjust</strong> setting in the <strong>Settings</strong> &gt; <strong>brightness</strong> screen.</p></td>
    </tr>
    <tr class="even">
    <td><p>1 or 'Hide'</p></td>
    <td><p>Use to hide the <strong>Automatically adjust</strong> setting in the <strong>Settings</strong> &gt; <strong>brightness</strong> screen.</p></td>
    </tr>
    </tbody>
    </table>

     

<a href="" id="testing-"></a>**Testing:**  
1.  Flash the build that contains this customization to a phone.

2.  In **Settings**, go to the **Brightness** screen.

3.  Verify that the **Automatically adjust** toggle is hidden or visible depending on the `Value` that you set for `HideAutoBrightness`.

 

 

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20%5Bp_phCustomization\p_phCustomization%5D:%20Hide%20the%20auto%20brightness%20setting%20%20RELEASE:%20%289/7/2016%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/default.aspx. "Send comments about this topic to Microsoft")




