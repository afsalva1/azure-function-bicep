# Set the environment variable to the desired environment (e.g. dev, qa, prod)
export environment=dev

# Deploy the Bicep file using the Azure CLI
az deployment sub create --location eastus --template-file ./azuredeploy.bicep --parameters environment=$environment
