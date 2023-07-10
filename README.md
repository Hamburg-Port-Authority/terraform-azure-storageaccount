# Introduction:

The module is used to deploy azure storageaccount over terraform with a default setup (Infrastructure as Code).

> **_NOTE:_** The required providers, providers configuration and terraform version are maintained in the user's configuration and are not maintained in the modules themselves.

# Example Use of Module:

    module "storageaccount" {

    source = "github.com/Hamburg-Port-Authority/terraform-azure-storageaccount?ref=1.0.1"

    name                = var.name
    resource_group_name = var.resource_group_name
    location            = var.location
    network_rules       = var.network_rules
    }
