## Login with 2FA

    $ az login --use-device-code --tenant 76c2d5a7-6e03-4b03-babd-f7149b110b4a

## Check and find the subsription id

  $ az account list

## Set default subscription

    $ az account set --subscription 909193c7-43c7-46c2-a4f5-061d7fe2eef6

## Check if subscription was set correctly

    $ az account show

## Create the resource group

    $ az group create --name rg-ais-<env>-001 --location westeurope

## Deploy the Landingzone

    $ cd deploy
    $ az deployment group create --resource-group rg-ais-<env>-001 --template-file deploy_ais_lz_<env>.json

