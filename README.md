# appgw-example

1. Create an RBAC that can create and manage resources. Tip: Run in Powershell.

`az ad sp create-for-rbac --name myApp --role contributor --scopes /subscriptions/{subscription-id} --sdk-auth`

2.  Save the output to GitHub Secret -> `AZURE_CREDENTIALS`

3.  Create an additional GitHub Secret called `AZURE_SUBSCRIPTION` with the subscription-id.
