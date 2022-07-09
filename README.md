# This Repo is to create and assign an Azure Blueprint that deploys a Storage Account Resource using Github Actions

### The Below Secrets need to be created to use Blueprint Create and Assign Action

| Secret_Name | Value |
| --- | ----------- |
| AZURETENANTID | Tenant ID of the Azure Subscrioption |
| AZURECLIENTID | Client ID of the Service Principal(App Registration) |
| AZUREPASSWORD | Client Secret of the Service Principal(App Registration) |
| AZURESUBSCRIPTIONID | Azure Subscription ID |


### Value to be replaced in the files for Deployment:

1. Blueprint.json
   - Replace the #### BLUEPRINT NAME #### with a suitable value

1. assign.json
   - Replace all the #### SUBSCRIPTION ID #### with your Subscription ID
   - Replcae the #### USER ASSIGNED IDENTITY NAME #### with your User Identity Name
   - Replace all #### LOCATION WITHOUT SPACES #### with your Resource Group Location (eg. eastus, westus)
   - Replace the #### BLUEPRINT NAME #### with the same value as give in the Blueprint.json
   - Replace the #### RESOURCE GROUP NAME #### with your Resource Group Name
   - Replcae the #### STORAGE ACCOUNT NAME (MUST BE UNIQUE) #### with the storage account name, it mus contain only alphanumeric char, no spaces, no special chars, not too long and must be unique

### Runtime Input Required

| Input_Name | Value |
| --- | ----------- |
| Blueprint_Name | Name of the Blueprint same as give in the Blueprint.json|
| Assignement_Name | Name of the blueprint Assignment (eg. assign-blueprintName) |

### Adding New Resources

IF you need to add a different resource you can use the sample-template.json in the Blueprints/AddOns folder and modify the parts marked with #### to add you template and parameters