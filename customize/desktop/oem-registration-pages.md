---
title: OEM registration pages
description: Add your OEM registration pages to OOBE
MSHAttr:
- 'PreferredSiteName:MSDN'
- 'PreferredLib:/library/windows/hardware'
ms.author: alhopper
ms.date: 01/23/2018
ms.topic: article
ms.prod: windows-hardware
ms.technology: windows-oem
---
# OEM registration pages

You can customize OEM registration pages to gather customer information, and introduce offers, during OOBE. If you choose to implement the optional registration pages, we recommend that you use them to provide information and opportunities that benefit your customers. The Windows 10 OOBE is designed to maximize customer engagement by creating pages that focus on one thing at a time. As a result, OEM registration fields are divided between two separate pages.

Here is an example of the two OEM registration pages:

![OEM registration page 1](images/oem-registration-page1.png)

![OEM registration page 2](images/oem-registration-page2.png)

The OEM registration pages work with the Microsoft Account (MSA) to help customers enter in their information only once during OOBE. Microsoft prompts customers to sign up for an MSA or sign into an existing MSA during OOBE. When a customer does this, their first name, last name, and email address for the MSA, if provided, will be pre-filled in on the OEM registration pages. The customer can change their information before clicking **Next** if desired.

If the customer has not used an MSA, the fields on the OEM registration pages will be empty, and the customer can fill them in if and as desired.

The OEM Registration pages are the last screens in the OOBE flow, after the user goes through all other steps in OOBE.

You can use an OEM App to collect and manage the customer information entered into the registration pages.

## In this section

The following topics describe how to add your registration pages to OOBE.

| Topic                                     | Description                                                                        |
|:------------------------------------------|:-----------------------------------------------------------------------------------|
| [Design your registration pages](design-registration-pages.md)   | Guidance on customizing the HTML of your registration pages. |
| [Configure OOBE.xml](registration-pages-oobexml.md)              | Create a custom Oobe.xml file or files as determined by the languages and regions where you ship your company's PCs. You can use multiple Oobe.xml files for language- and region-specific terms and settings so users see the correct language as soon as they start their PCs. You must provide a page title, a page subtitle, a consent statement description, and at least one labeled screen element (for example, one of the input fields) to display the registration pages.                         |
| [Manage and upload user data](manage-user-data.md)               | Generate a public/private key pair for customer data encryption and decryption. To protect customer privacy, Windows encrypts the customer data that's generated through participation in, and completion of, the Registration pages. If the OEM doesn't store a public key appropriately, the Registration pages aren't shown.     |
| [Collect and upload data](collect-and-upload-data.md)            | Create and preinstall a Microsoft Store app, or write a service to run after first sign-in, to collect the encrypted customer data, and upload that data set to your server for decryption and use. |
