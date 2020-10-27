# Deploy resource group into Azure

This template allows you to create a resource group in Customer Environment.

NOTE:  To deploy to a subscription, use the subscription-level deployment commands.


## Deployment

1. Using Azure CLI

  https://azure.microsoft.com/en-us/documentation/articles/xplat-cli-azure-resource-manager/

Example:

az deployment sub create \
  --name demoSubDeployment \
  --location centralus \
  --template-uri "https://raw.githubusercontent.com/Azure/azure-docs-json-samples/master/azure-resource-manager/emptyRG.json" \
  --parameters rgName=demoResourceGroup rgLocation=centralus
  
