<!-- BEGIN_TF_DOCS -->
## Requirements

The following requirements are needed by this module:

- <a name="requirement_terraform"></a> [terraform](#requirement\_terraform) (>= 1.10.3)

- <a name="requirement_azurerm"></a> [azurerm](#requirement\_azurerm) (~> 4.14)

## Providers

The following providers are used by this module:

- <a name="provider_azurerm"></a> [azurerm](#provider\_azurerm) (~> 4.14)

- <a name="provider_random"></a> [random](#provider\_random)

## Modules

No modules.

## Resources

The following resources are used by this module:

- [azurerm_key_vault.kv](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/resources/key_vault) (resource)
- [azurerm_resource_group.rg](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/resources/resource_group) (resource)
- [azurerm_user_assigned_identity.uai](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/resources/user_assigned_identity) (resource)
- [random_integer.kv_num](https://registry.terraform.io/providers/hashicorp/random/latest/docs/resources/integer) (resource)
- [azurerm_client_config.current](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/data-sources/client_config) (data source)

## Required Inputs

The following input variables are required:

### <a name="input_key_vault_name"></a> [key\_vault\_name](#input\_key\_vault\_name)

Description: Specifies a key vault name

Type: `string`

### <a name="input_resource_group_name"></a> [resource\_group\_name](#input\_resource\_group\_name)

Description: Specifies the name of the resource group that will be created.

Type: `string`

### <a name="input_tags"></a> [tags](#input\_tags)

Description: Specifies a map of tags to be applied to the resources created.

Type: `map(any)`

## Optional Inputs

The following input variables are optional (have default values):

### <a name="input_location"></a> [location](#input\_location)

Description: The location/region where Azure resource will be created.

Type: `string`

Default: `"uksouth"`

### <a name="input_use_rbac_mode"></a> [use\_rbac\_mode](#input\_use\_rbac\_mode)

Description: Specifies to use rbac mode. (Optional)

Type: `bool`

Default: `null`

## Outputs

No outputs.
<!-- END_TF_DOCS -->