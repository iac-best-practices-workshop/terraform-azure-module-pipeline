# Mario mendes

# terraform-azure-module-pipeline

About
Repository used to train CI/CD and Release strategies

## Instructions

You should fork this project and test / experiment different release strategies (Trunk-Based, Git Flow, Release Bases).

## Requirements

No requirements.

## Providers

| Name                                                         | Version |
| ------------------------------------------------------------ | ------- |
| <a name="provider_azurerm"></a> [azurerm](#provider_azurerm) | n/a     |

## Modules

No modules.

## Resources

| Name                                                                                                                               | Type     |
| ---------------------------------------------------------------------------------------------------------------------------------- | -------- |
| [azurerm_storage_account.example](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/resources/storage_account) | resource |

## Inputs

| Name                                                                                                      | Description                                                                                               | Type     | Default      | Required |
| --------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------- | -------- | ------------ | :------: |
| <a name="input_account_name"></a> [account_name](#input_account_name)                                     | The name of the storage account                                                                           | `string` | n/a          |   yes    |
| <a name="input_account_replication_type"></a> [account_replication_type](#input_account_replication_type) | Defines the type of replication to use for this storage account (LRS / GRS / RAGRS / ZRS / GZRS / RAGZRS) | `string` | `"LRS"`      |    no    |
| <a name="input_account_tier"></a> [account_tier](#input_account_tier)                                     | Defines the Tier to use for this storage account (Standard / Premium)                                     | `string` | `"Standard"` |    no    |
| <a name="input_location"></a> [location](#input_location)                                                 | The location/region where the storage account is created                                                  | `string` | n/a          |   yes    |
| <a name="input_resource_group_name"></a> [resource_group_name](#input_resource_group_name)                | The name of the resource group in which to create the storage account                                     | `string` | n/a          |   yes    |

## Outputs

| Name                                                                                                                                                           | Description                                           |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------- |
| <a name="output_storage_account_name"></a> [storage_account_name](#output_storage_account_name)                                                                | The name of the storage account                       |
| <a name="output_storage_account_primary_connection_string"></a> [storage_account_primary_connection_string](#output_storage_account_primary_connection_string) | The primary connection string for the storage account |
