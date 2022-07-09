# This Repo is to create and assign an Azure Blueprint that deploys a Storage Account Resource using Github Actions

The Below Secrets need to be created to use Blueprint Create and Assign Action

| Secret_Name | Value |
| --- | ----------- |
| AZURETENANTID | Tenant ID of the Azure Subscrioption |
| AZURECLIENTID | Client ID of the Service Principal(App Registration) |
| AZUREPASSWORD | Client Secret of the Service Principal(App Registration) |
| AZURESUBSCRIPTIONID | Azure Subscription ID |


Runtime Input Required

| Input_Name | Value |
| --- | ----------- |
| Blueprint_Name | Name of the Blueprint |
| Assignement_Name | Name of the blueprint Assignment (Can be just assig-blueprintName) |