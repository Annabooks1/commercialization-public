---
title: Group
description: Group
MSHAttr:
- 'PreferredSiteName:MSDN'
- 'PreferredLib:/library/windows/hardware'
ms.assetid: 08f9c3ed-d6e1-4950-aa4c-fcf04680c387
ms.prod: W10
ms.mktglfcycl: deploy
ms.sitesec: msdn
---

# Group


`Group` specifies the local security group to which the domain account or the security group will be added. You can add a user to multiple groups by entering multiple group names separated by semicolons.

The [Microsoft-Windows-Shell-Setup](microsoft-windows-shell-setup.md) component recognizes the following English group names and sets the appropriate localized group name, regardless of the default language of the Windows image:

-   AccountOperators

-   Administrators

-   BackupOperators

-   CryptoOperators

-   DCOMUsers

-   Guests

-   IUsers

-   NetworkConfigurationOperators

-   PerfLoggingUsers

-   PerfMonitoringUsers

-   PowerUsers

-   PrintOperators

-   RemoteDesktopUsers

-   Replicator

-   SystemOperators

-   Users

Specify the account names and group names by using language-neutral names. The language-neutral account and group names are specified in English—for example, **Administrators**, **Power Users**, and **Guest**. This is required because the shell account settings are processed before a default user interface (UI) language is applied to the computer.

## Values


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><em>Group_name</em></p></td>
<td><p>Specifies the local security group to which the domain account or the security group will be added. More than one group can be specified (separated by semicolons). <em>Group_name</em> is a string with a maximum length of 256 characters.</p></td>
</tr>
</tbody>
</table>

 

This string type supports empty elements.

## Valid Passes


auditSystem

oobeSystem

## Parent Hierarchy


[Microsoft-Windows-Shell-Setup](microsoft-windows-shell-setup.md) | [UserAccounts](microsoft-windows-shell-setupuseraccounts.md) | [DomainAccounts](microsoft-windows-shell-setupuseraccountsdomainaccounts.md) | [DomainAccountList](microsoft-windows-shell-setupuseraccountsdomainaccountsdomainaccountlist.md) | [DomainAccount](microsoft-windows-shell-setupuseraccountsdomainaccountsdomainaccountlistdomainaccount.md) | **Group**

## Applies To


For a list of the supported Windows editions and architectures that this component supports, see [Microsoft-Windows-Shell-Setup](microsoft-windows-shell-setup.md).

## XML Example


The following XML examples show how to use the **Group** setting to add domain groups to local security groups.

Example 1:

``` syntax
<DomainAccounts>
   <DomainAccountList wcm:action="add">
      <DomainAccount wcm:action="add">
        <Group>Users</Group> 
        <Name>Domain Users</Name> 
      </DomainAccount>
   <Domain>FabrikamDomain</Domain> 
   </DomainAccountList>
</DomainAccounts>
```

Example 2:

``` syntax
<DomainAccounts>
   <DomainAccountList wcm:action="add">
      <DomainAccount wcm:action="add">
        <Group>Administrators</Group> 
        <Name>Domain Administrators</Name> 
      </DomainAccount>
   <Domain>FabrikamDomain</Domain> 
   </DomainAccountList>
</DomainAccounts>
```

## Related topics


[DomainAccount](microsoft-windows-shell-setupuseraccountsdomainaccountsdomainaccountlistdomainaccount.md)

 

 

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20%5Bp_unattend\p_unattend%5D:%20Group%20%20RELEASE:%20%2810/3/2016%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/default.aspx. "Send comments about this topic to Microsoft")





