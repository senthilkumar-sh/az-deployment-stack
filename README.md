# az-deployment-stack

Deployment Stack
az stack group create --name Res-Grp-stack -g xyz-res-grp --deny-settings-mode 'none' --template-file deployment-stacks.json

az stack group create --name Res-Grp-stack -g abc-res-grp --deny-settings-mode 'none' --template-file deploy-rg-stg-stack.json


az stack sub create --name Sub-Stack --template-file deploy-sub-stack.json -l westus --deny-settings-mode 'none' 


az stack mg create -m Contoso100 -n Mg-Stack --template-file deploy-mg-stack.json --location westus --parameters subscriptionID=<SUB_ID> --deny-settings-mode 'None'


