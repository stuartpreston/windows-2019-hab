# Windows 2019 with Habitat support

This Azure Resource Manager (ARM) template will create a Windows 2019 machine with Habitat correctly configured at first login.
It uses public (internet-accessible) resources, so will not work in an "air-gapped" environment.

## Quickstart

```bash
az login
az account set --subscription 43706c4e-YOUR-SUBS-HERE-e64e6bf63ac4
az group create --location northeurope --name yourname-hab-testing
az group deployment create -g yourname-hab-testing --template-file azuredeploy.json --parameters @azuredeploy.parameters.json
```
