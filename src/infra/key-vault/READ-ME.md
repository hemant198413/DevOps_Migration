# Keyvault Deployment

Templates for the SiteCore AKS Cluster deployment

Dev  CLI Commands:

Dry-Run

az deployment group what-if --name "local-what-if-keyvault"  --template-file group-template.json --parameters group-template-params.json --parameters engineerADGroupPrincipalId=7e252e01-75d2-44a4-baed-eeea715784c1 logWorkspacesName=app-log-analytics-eastus2-sttu2yxqow6r6 servicePrincipleDevOps=7de42fce-a6d0-458c-8d2e-406798a11153 pooldbname=cdprpi hyperdbname=cdphyps environment=dev --resource-group hips-cdp-eastus2 --subscription "hips-cdp-dev"

az deployment group what-if --name "local-what-if-keyvault"  --template-file group-template.json --parameters group-template-params.json --parameters engineerADGroupPrincipalId=13b21308-7a6d-42f5-bae8-d9fa42df8501 servicePrincipleDevOps=7de42fce-a6d0-458c-8d2e-406798a11153 --resource-group hips-cdp-eastus2 --subscription "hips-cdp-test"

az deployment group what-if --name "local-what-if-keyvault"  --template-file group-template.json --parameters group-template-params.json --parameters engineerADGroupPrincipalId=f65b27be-51b7-416a-9fde-847fea6546eb logWorkspacesName=app-log-analytics-eastus2-rl5cemakajfpc servicePrincipleDevOps=7de42fce-a6d0-458c-8d2e-406798a11153 pooldbname=cdprpis hyperdbname=cdphypss environment=preprod --resource-group hips-cdp-eastus2 --subscription "hips-cdp-preprod"

az deployment group what-if  --name "local-what-if-group-keyvault"  --template-file group-template.json --parameters group-template-params.json --parameters engineerADGroupPrincipalId=42907c92-0cee-4667-b44d-98c7547e5ad8 servicePrincipleDevOps=7de42fce-a6d0-458c-8d2e-406798a11153 --resource-group hips-cdp-eastus2 --subscription "hips-cdp-prod"

Deploy
az deployment group create --name "local-deploy-group-keyvault"  --template-file group-template.json --parameters group-template-params.json --parameters engineerADGroupPrincipalId=7e252e01-75d2-44a4-baed-eeea715784c1 logWorkspacesName=app-log-analytics-eastus2-sttu2yxqow6r6 servicePrincipleDevOps=7de42fce-a6d0-458c-8d2e-406798a11153 pooldbname=cdprpi hyperdbname=cdphyps environment=dev --resource-group hips-cdp-eastus2 --subscription "hips-cdp-dev"

az deployment group create --name "local-deploy-group-keyvault"  --template-file group-template.json --parameters group-template-params.json --parameters engineerADGroupPrincipalId=13b21308-7a6d-42f5-bae8-d9fa42df8501 servicePrincipleDevOps=7de42fce-a6d0-458c-8d2e-406798a11153 --resource-group hips-cdp-eastus2 --subscription "hips-cdp-test"

az deployment group create --name "local-deploy-group-keyvault"   --template-file group-template.json --parameters group-template-params.json --parameters engineerADGroupPrincipalId=f65b27be-51b7-416a-9fde-847fea6546eb logWorkspacesName=app-log-analytics-eastus2-rl5cemakajfpc servicePrincipleDevOps=7de42fce-a6d0-458c-8d2e-406798a11153 pooldbname=cdprpis hyperdbname=cdphypss environment=preprod --resource-group hips-cdp-eastus2 --subscription "hips-cdp-preprod"

az deployment group create --name "local-deploy-group-keyvault"  --template-file group-template.json --parameters group-template-params.json --parameters engineerADGroupPrincipalId=f65b27be-51b7-416a-9fde-847fea6546eb servicePrincipleDevOps=7de42fce-a6d0-458c-8d2e-406798a11153 --resource-group hips-cdp-eastus2 --subscription "hips-cdp-preprod"

az deployment group create --name "local-deploy-group-keyvault"  --template-file group-template.json --parameters group-template-params.json --parameters engineerADGroupPrincipalId=42907c92-0cee-4667-b44d-98c7547e5ad8 servicePrincipleDevOps=7de42fce-a6d0-458c-8d2e-406798a11153 --resource-group hips-cdp-eastus2 --subscription "hips-cdp-prod"


## Assignments