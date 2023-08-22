# Epac2 Policy effects 

Auto-generated Policy effect documentation across environments 'prod' sorted by Policy category and Policy display name.

## Table of contents

- [Environments](#environments)
- [Policy effects across environments](#policy-effects-across-environment)

## <a id="environments"></a>Environments


### **prod environment**

Scopes

- Management Group: EPAC-Dev2

Assignment 

- PolicySet: Global initiative general
- Type: Custom
- Category: General
- Description: This initiative contains the general policies valid to the entire OTG platform, such as naming and tagging conventions and limits for Azure region deployments.

<br/>

## <a id='policy-effects-across-environment'></a>Policy effects across environment

<br/>

| Category | Policy | prod |
| :------- | :----- | :-----: |
| General | **Allowed locations**<br/>This policy enables you to restrict the locations your organization can specify when deploying resources. Use to enforce your geo-compliance requirements. Excludes resource groups, Microsoft.AzureActiveDirectory/b2cDirectories, and resources that use the 'global' region. |  ***deny*** |
| General | **Allowed locations for resource groups**<br/>This policy enables you to restrict the locations your organization can create resource groups in. Use to enforce your geo-compliance requirements. |  ***deny*** |
| General | **Append createdDate to resource group**<br/>Tags deployed resource groups with date time in utc format using append action, if it is missing. Does not modify other tags and is very simple: when used in an environment where no resources exist prior, it will ensure that all resource groups have the createdDate tag value. Therefore the value will not be updated when a resource group is updated, as the exists condition will be true. |  **Append**<br/>*Disabled*<br/>*Audit*<br/>*Deny* |
| General | **Enforce naming convention**<br/>This policy ensures that all resources are named according to the naming convention. |  **Deny**<br/>*Disabled*<br/>*Audit* |
| Sandbox | **append-rg-deleteDate**<br/>Tags deployed resource groups with date time in utc format using append action, if it is missing. Does not modify other tags and is very simple: when used in an environment where no resources exist prior, it will ensure that all resource groups have the createdDate tag value. Therefore the value will not be updated when a resource group is updated, as the exists condition will be true. |  **Disabled**<br/>*Audit*<br/>*Deny* |
| Sandbox | **Deny vNet peer creation**<br/>This policy denies the creation of vNet Peerings under the assigned scope |  **Disabled**<br/>*Audit*<br/>*Deny* |
| Sandbox | **Deny vNet peering creation cross subscription**<br/>This policy denies the creation of vNet Peerings across subscriptions. |  **Disabled**<br/>*Audit*<br/>*Deny* |
