# Web App Deployment

Templates for the Hips-CDP Web App Cluster deployment

Dev  CLI Commands:

#HIPS-CDP-DEV
    Dry-Run
    az deployment group what-if --name "local-what-if-group-webapp"  --template-file group-template.json --parameters group-template-params.json --parameter environment=dev --resource-group hips-cdp-eastus2 --subscription "hips-cdp-dev"

    Deploy
     az deployment group create --name "local-create-group-webapp"  --template-file group-template.json --parameters group-template-params.json --parameter environment=dev --resource-group hips-cdp-eastus2 --subscription "hips-cdp-dev"

#HIPS-CDP-TEST
    Dry-Run
    az deployment group what-if --name "local-what-if-group-webapp"  --template-file group-template.json --parameters group-template-params.json --parameter webAppName=rgitestrpisite existingVirtualNetworkName=vnet-hips-cdp-test-eastus2 environment=test --resource-group hips-cdp-eastus2 --subscription "hips-cdp-test"

    Deploy
    az deployment group create --name "local-deploy-group-webapp"  --template-file group-template.json --parameters group-template-params.json --parameter webAppName=rgitestrpisite existingVirtualNetworkName=vnet-hips-cdp-test-eastus2 environment=test --resource-group hips-cdp-eastus2 --subscription "hips-cdp-test"


#HIPS-CDP-PROProd
    Dry-Run
    az deployment group what-if --name "local-what-if-group-webapp"  --template-file group-template.json --parameters group-template-params.json --parameter environment=preprod existingVirtualNetworkName=vnet-hips-cdp-preprod-eastus2 privateDnsZonesName=redpoint.preprod.azure.mskcc.org certificateThumbPrint=D4C533BCAF1171C6C08B161AFE92F6610DEAB855 --resource-group hips-cdp-eastus2 --subscription "hips-cdp-preprod"

    Deploy
   az deployment group create --name "local-deploy-group-webapp"  --template-file group-template.json --parameters group-template-params.json --parameter environment=preprod existingVirtualNetworkName=vnet-hips-cdp-preprod-eastus2 privateDnsZonesName=redpoint.preprod.azure.mskcc.org certificateThumbPrint=D4C533BCAF1171C6C08B161AFE92F6610DEAB855 --resource-group hips-cdp-eastus2 --subscription "hips-cdp-preprod"

#HIPS-CDP-Prod
    Dry-Run
    az deployment group what-if --name "local-what-if-group-webapp"  --template-file group-template.json --parameters group-template-params.json --parameter environment=prod existingVirtualNetworkName=vnet-hips-cdp-prod-eastus2 privateDnsZonesName=redpoint.azure.mskcc.org certificateThumbPrint=0544945B5F96BE8876034B155D1163E20EBD4F9D --resource-group hips-cdp-eastus2 --subscription "hips-cdp-prod"

    Deploy
   az deployment group create --name "local-deploy-group-webapp"  --template-file group-template.json --parameters group-template-params.json --parameter environment=prod existingVirtualNetworkName=vnet-hips-cdp-prod-eastus2 privateDnsZonesName=redpoint.azure.mskcc.org certificateThumbPrint=0544945B5F96BE8876034B155D1163E20EBD4F9D   --resource-group hips-cdp-eastus2 --subscription "hips-cdp-prod"

## Assignments
