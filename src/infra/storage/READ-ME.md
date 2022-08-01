# demo Deployment

Templates for the storage deployment

Dev  CLI Commands:


"hips-cdp-dev"

```shell 
# Preview dev
    # Dry-Run
        
    az deployment group what-if --name "local-what-if-demo-st"  --template-file group-template.json --parameters group-template-params.json --parameters storageAccounts_name=de2 --resource-group hips-cdp-eastus2 --subscription "hips-cdp-dev"

    # Deploy

    az deployment group create --name "local-create-demo-st"  --template-file group-template.json --parameters group-template-params.json --parameters storageAccounts_name=de2 --resource-group hips-cdp-eastus2 --subscription "hips-cdp-dev"

```