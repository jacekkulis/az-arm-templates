# Azure quicksart ARM templates
This folder contains sample templates that can be used to quickly provision a single or set of resources to for the purposes of evaluating the infrastructure. Many of these samples are also used as canonical examples for documentation.

For for more information see the documentation [here](https://github.com/Azure/azure-quickstart-templates).

# Prerequisites

## Create resource group if needed

**Azure CLI**
```
  az group create --subscription <subscription_id> -l <location> -n <resource_group_name> --tags <optional_tags>
```

## Deployment

**Azure CLI**
```
  az group deployment create --name <deployment_display_name> --resource-group <resource_group_name --template-uri <uri> --parameters contactEmails="['email@address.com', 'email2@address.com']"
```

or 

```
  az group deployment create --name <deployment_display_name> --resource-group <resource_group_name --template-file <file_path> --parameters <file_path>
```
