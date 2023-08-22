# Document Initiatives

Auto-generated Policy effect documentation for PolicySets grouped by Effect and sorted by Policy category and Policy display name.

## Table of contents

- [PolicySets](#policySets)
- [Policies](#policies)

<br/>

## <a id="policySets"></a>PolicySets

### global-general

- Display name: Global initiative general
- Type: Custom
- Category: General

This initiative contains the general policies valid to the entire OTG platform, such as naming and tagging conventions and limits for Azure region deployments.

### vnet-peering-sandbox

- Display name: Sandbox initiative
- Type: Custom
- Category: Sandbox

Security controls for sandbox, such as denial of vnet creation.


<br/>

## <a id='policies'></a>Policies

<br/>

| Category | Policy | global-general | vnet-peering-sandbox |
| :------- | :----- | :-------- | :-------- |
| General | **Allowed locations**<br/>This policy enables you to restrict the locations your organization can specify when deploying resources. Use to enforce your geo-compliance requirements. Excludes resource groups, Microsoft.AzureActiveDirectory/b2cDirectories, and resources that use the 'global' region.<br/>*Global initiative general:*<br/>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*AllowedLocations = `++ no default ++`* | ***deny*** |  |
| General | **Allowed locations for resource groups**<br/>This policy enables you to restrict the locations your organization can create resource groups in. Use to enforce your geo-compliance requirements.<br/>*Global initiative general:*<br/>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*AllowedLocations = `++ no default ++`* | ***deny*** |  |
| General | **Append createdDate to resource group**<br/>Tags deployed resource groups with date time in utc format using append action, if it is missing. Does not modify other tags and is very simple: when used in an environment where no resources exist prior, it will ensure that all resource groups have the createdDate tag value. Therefore the value will not be updated when a resource group is updated, as the exists condition will be true. | **Append**<br/>*Audit*<br/>*Deny*<br/>*Disabled* |  |
| General | **Enforce naming convention**<br/>This policy ensures that all resources are named according to the naming convention. | **Deny**<br/>*Audit*<br/>*Disabled* |  |
| Sandbox | **append-rg-deleteDate**<br/>Tags deployed resource groups with date time in utc format using append action, if it is missing. Does not modify other tags and is very simple: when used in an environment where no resources exist prior, it will ensure that all resource groups have the createdDate tag value. Therefore the value will not be updated when a resource group is updated, as the exists condition will be true.<br/>*Sandbox initiative:*<br/>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*effect = `Disabled`* |  | **Disabled**<br/>*Audit*<br/>*Deny* |
| Sandbox | **Deny vNet peer creation**<br/>This policy denies the creation of vNet Peerings under the assigned scope<br/>*Sandbox initiative:*<br/>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*effect = `Disabled`* |  | **Disabled**<br/>*Audit*<br/>*Deny* |
| Sandbox | **Deny vNet peering creation cross subscription**<br/>This policy denies the creation of vNet Peerings across subscriptions.<br/>*Sandbox initiative:*<br/>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*effect = `Disabled`* |  | **Disabled**<br/>*Audit*<br/>*Deny* |
