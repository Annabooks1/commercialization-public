---
title: EnterpriseModernAppManagement XSD
description: Here is the XSD for the application parameters.
MSHAttr:
- 'PreferredSiteName:MSDN'
- 'PreferredLib:/library/windows/hardware'
ms.assetid: D393D094-25E5-4E66-A60F-B59CC312BF57
ms.author: windows-hardware-design-content
ms.date: 05/02/2017
ms.topic: article
ms.prod: windows-hardware
ms.technology: windows-oem
---

# EnterpriseModernAppManagement XSD


Here is the XSD for the application parameters.

``` syntax
<?xml version="1.0" encoding="utf-16"?>
<xs:schema attributeFormDefault="unqualified" elementFormDefault="qualified" xmlns:xs="http://www.w3.org/2001/XMLSchema">
    <xs:element name="Data">
        <xs:complexType>
            <xs:sequence>
                <xs:element maxOccurs="1" name="Application">
                    <xs:complexType mixed="true">
                        <xs:sequence minOccurs="0">
                            <xs:element name="Dependencies">
                                <xs:complexType>
                                    <xs:sequence>
                                        <xs:element maxOccurs="unbounded" name="Dependency">
                                            <xs:complexType>
                                                <xs:attribute name="PackageUri" type="xs:string" use="required" />
                                            </xs:complexType>
                                        </xs:element>
                                    </xs:sequence>
                                </xs:complexType>
                            </xs:element>
                        </xs:sequence>
                        <xs:attribute name="DeploymentOptions" type="xs:unsignedByte" use="optional" />
                        <xs:attribute name="PackageUri" type="xs:string" use="required" />
                    </xs:complexType>
                </xs:element>
            </xs:sequence>
        </xs:complexType>
    </xs:element>
</xs:schema>
```

 

 






