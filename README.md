#README

This is a JSON Template for creating Azure RBAC custom role definition

##Create custom role definition

New-AzRoleDefinition -InputFile "pathToJSONTemplate"

##Assign role definition

New-AzRoleAssignment -ResourceGroupName rg1 -SignInName demo@email.com -RoleDefinitionName Reader -AllowDelegation

##Reference
https://docs.microsoft.com/en-us/powershell/module/az.resources/new-azroleassignment?view=azps-1.8.0