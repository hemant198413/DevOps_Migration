# AKS Deployment

Templates for the Hips-CDP AKS Cluster deployment

CLI Commands:

# hips-cdp-dev 
    Dry-Run

```
az deployment group what-if --name "local-what-if-group-private-aks"  --template-file group-template.json --parameters group-template-params.json --parameters engineerADGroupPrincipalId=7e252e01-75d2-44a4-baed-eeea715784c1 tenantID=93c5fcb5-2df6-4550-9a10-cd35f285cf7c logWorkspacesName=app-log-analytics-eastus2-sttu2yxqow6r6 existingVirtualNetworkName=vnet-hips-cdp-dev-eastus2 dnsServiceIP=100.64.0.20 keyEncryptionKeyURL='https://kv-sc-2orig5io4dka2.vault.azure.net/keys/hips-disk-encryption-key/4860486b31b34a8782543a2ec03c3c97' --resource-group hips-cdp-eastus2 --subscription "hips-cdp-dev"

```
Deploy

```
az deployment group create --name "local-deploy-group-private-aks"  --template-file group-template.json --parameters group-template-params.json --parameters engineerADGroupPrincipalId=7e252e01-75d2-44a4-baed-eeea715784c1 tenantID=93c5fcb5-2df6-4550-9a10-cd35f285cf7c logWorkspacesName=app-log-analytics-eastus2-sttu2yxqow6r6 existingVirtualNetworkName=vnet-hips-cdp-dev-eastus2 dnsServiceIP=100.64.0.20 keyEncryptionKeyURL='https://kv-sc-2orig5io4dka2.vault.azure.net/keys/hips-disk-encryption-key/4860486b31b34a8782543a2ec03c3c97' --resource-group hips-cdp-eastus2 --subscription "hips-cdp-dev"

```
# hips-cdp-test 
    Dry-Run

```

az deployment group what-if --name "local-what-if-group-private-aks" --template-file group-template.json --parameters group-template-params.json --parameters engineerADGroupPrincipalId=13b21308-7a6d-42f5-bae8-d9fa42df8501 tenantID=93c5fcb5-2df6-4550-9a10-cd35f285cf7c logWorkspacesName=app-log-analytics-eastus2-w6oebtt5ql2ku existingVirtualNetworkName=vnet-hips-cdp-test-eastus2 dnsServiceIP=100.64.0.30 keyEncryptionKeyURL='https://kv-sc-2urinqzb6seg4.vault.azure.net/keys/hips-disk-encryption-key/ad8beaae7d3749d4a1e9cf840b873317' --resource-group hips-cdp-eastus2 --subscription "hips-cdp-test"

```
Deploy

```
az deployment group create --name "local-deploy-group-private-aks" --template-file group-template.json --parameters group-template-params.json --parameters engineerADGroupPrincipalId=13b21308-7a6d-42f5-bae8-d9fa42df8501 tenantID=93c5fcb5-2df6-4550-9a10-cd35f285cf7c logWorkspacesName=app-log-analytics-eastus2-w6oebtt5ql2ku existingVirtualNetworkName=vnet-hips-cdp-test-eastus2 dnsServiceIP=100.64.0.30 keyEncryptionKeyURL='https://kv-sc-2urinqzb6seg4.vault.azure.net/keys/hips-disk-encryption-key/ad8beaae7d3749d4a1e9cf840b873317' --resource-group hips-cdp-eastus2 --subscription "hips-cdp-test"

```

# hips-cdp-preprod 

Dry-Run

```

az deployment group what-if --name "local-what-if-group-private-aks" --template-file group-template.json --parameters group-template-params.json --parameters engineerADGroupPrincipalId=f65b27be-51b7-416a-9fde-847fea6546eb tenantID=93c5fcb5-2df6-4550-9a10-cd35f285cf7c logWorkspacesName=app-log-analytics-eastus2-rl5cemakajfpc existingVirtualNetworkName=vnet-hips-cdp-preprod-eastus2 dnsServiceIP=100.64.0.60 keyEncryptionKeyURL='https://kv-sc-l2r5n62jaa7l2.vault.azure.net/keys/hips-disk-encryption-key/3e7ac83667b5459d828f5c1cadb69ddb' --resource-group hips-cdp-eastus2 --subscription "hips-cdp-preprod"

```
Deploy

```
az deployment group create --name "local-deploy-group-private-aks" --template-file group-template.json --parameters group-template-params.json --parameters engineerADGroupPrincipalId=f65b27be-51b7-416a-9fde-847fea6546eb tenantID=93c5fcb5-2df6-4550-9a10-cd35f285cf7c logWorkspacesName=app-log-analytics-eastus2-rl5cemakajfpc existingVirtualNetworkName=vnet-hips-cdp-preprod-eastus2 dnsServiceIP=100.64.0.60 keyEncryptionKeyURL='https://kv-sc-l2r5n62jaa7l2.vault.azure.net/keys/hips-disk-encryption-key/3e7ac83667b5459d828f5c1cadb69ddb' --resource-group hips-cdp-eastus2 --subscription "hips-cdp-preprod"
```

# hips-cdp-prod 

Dry-Run

```

az deployment group what-if --name "local-what-if-group-private-aks" --template-file group-template.json --parameters group-template-params.json --parameters engineerADGroupPrincipalId=42907c92-0cee-4667-b44d-98c7547e5ad8 tenantID=93c5fcb5-2df6-4550-9a10-cd35f285cf7c logWorkspacesName=app-log-analytics-eastus2-ymxt7sbis6fac existingVirtualNetworkName=vnet-hips-cdp-prod-eastus2 dnsServiceIP=100.64.0.80 keyEncryptionKeyURL='https://kv-sc-t2asvyx3g5mio.vault.azure.net/keys/hips-disk-encryption-key/941791f1481f4512b235231c918ad850' --resource-group hips-cdp-eastus2 --subscription "hips-cdp-prod"

```
Deploy

```
az deployment group create --name "local-deploy-group-private-aks" --template-file group-template.json --parameters group-template-params.json --parameters engineerADGroupPrincipalId=42907c92-0cee-4667-b44d-98c7547e5ad8 tenantID=93c5fcb5-2df6-4550-9a10-cd35f285cf7c logWorkspacesName=app-log-analytics-eastus2-ymxt7sbis6fac existingVirtualNetworkName=vnet-hips-cdp-prod-eastus2 dnsServiceIP=100.64.0.80 keyEncryptionKeyURL='https://kv-sc-t2asvyx3g5mio.vault.azure.net/keys/hips-disk-encryption-key/941791f1481f4512b235231c918ad850' --resource-group hips-cdp-eastus2 --subscription "hips-cdp-prod"

```

## Assignments
