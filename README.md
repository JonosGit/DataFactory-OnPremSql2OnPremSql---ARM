# DataFactory-OnPremSql2OnPremSql---ARM


DataFactoryOnPremSql2OnPremSql.json - ARM Template to deploy OnPrem SQL to OnPrem SQL Pipeline
DataFactoryOnPremSql2OnPrem_Answer.json - ARM Answer File to automate DataFactoryOnPremSql2OnPrem.json deployment

To Execute the template run the following commands in Azure Powershell 1.x or greater after downloading the ARM template to C:\Temp. Note you will need to update the Template Parameter File if you decide to use it.

Login-AzureRMAccount
New-AzureRmResourceGroup -Location "WESTUS" -Name "DataFactory"

New-AzureRmResourceGroupDeployment -ResourceGroupName "DataFactory" -TemplateFile C:\Temp\DataFactoryOnPremtoSqlAzure.json -TemplateParameterFile C:\Temp\DataFactoryARM_Answer.json
-