
# Enterprise application

Creates an enterprise application as contributor role to run the inline scanning acr task.


<!-- BEGINNING OF PRE-COMMIT-TERRAFORM DOCS HOOK -->
## Requirements

| Name | Version |
|------|---------|
| <a name="requirement_terraform"></a> [terraform](#requirement\_terraform) | >= 0.15.0 |
| <a name="requirement_azuread"></a> [azuread](#requirement\_azuread) | 2.7.0 |
| <a name="requirement_azurerm"></a> [azurerm](#requirement\_azurerm) | >=3.52.0 |

## Providers

| Name | Version |
|------|---------|
| <a name="provider_azuread"></a> [azuread](#provider\_azuread) | 2.7.0 |
| <a name="provider_azurerm"></a> [azurerm](#provider\_azurerm) | 3.48.0 |

## Modules

No modules.

## Resources

| Name | Type |
|------|------|
| [azuread_application.aa](https://registry.terraform.io/providers/hashicorp/azuread/2.7.0/docs/resources/application) | resource |
| [azuread_application_password.aap](https://registry.terraform.io/providers/hashicorp/azuread/2.7.0/docs/resources/application_password) | resource |
| [azuread_service_principal.asp](https://registry.terraform.io/providers/hashicorp/azuread/2.7.0/docs/resources/service_principal) | resource |
| [azuread_service_principal_password.aspp](https://registry.terraform.io/providers/hashicorp/azuread/2.7.0/docs/resources/service_principal_password) | resource |
| [azurerm_role_assignment.main](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/resources/role_assignment) | resource |
| [azurerm_role_definition.ard](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/resources/role_definition) | resource |
| [azuread_client_config.current](https://registry.terraform.io/providers/hashicorp/azuread/2.7.0/docs/data-sources/client_config) | data source |

## Inputs

| Name | Description | Type | Default | Required |
|------|-------------|------|---------|:--------:|
| <a name="input_name"></a> [name](#input\_name) | Name to be assigned to all child resources. A suffix may be added internally when required. Use default value unless you need to install multiple instances | `string` | n/a | yes |
| <a name="input_subscription_ids"></a> [subscription\_ids](#input\_subscription\_ids) | Subscription IDs for apply the service principal scope | `list(string)` | n/a | yes |

## Outputs

| Name | Description |
|------|-------------|
| <a name="output_client_id"></a> [client\_id](#output\_client\_id) | Service principal ID |
| <a name="output_client_secret"></a> [client\_secret](#output\_client\_secret) | Service principal secret |
| <a name="output_tenant_id"></a> [tenant\_id](#output\_tenant\_id) | Service principal tenant ID |
<!-- END OF PRE-COMMIT-TERRAFORM DOCS HOOK -->

## Authors

Module is maintained and supported by [Sysdig](https://sysdig.com).

## License

Apache 2 Licensed. See LICENSE for full details.
