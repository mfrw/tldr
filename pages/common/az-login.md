# az login

> Login to Azure.
> Part of `az`.
> More information: <https://docs.microsoft.com/cli/azure/login>.

- Login interactively:

`az login`

- Login with a username and password:

`az login --username {{alias@somedomain.com}} --password {{secret}}`

- Login with a service principal using client secret:

`az login --service-principal --username {{http://azure-cli-service-principal}} --passsword {{secret}} --tenant {{someone.onmicrosoft.com}}`

- Login with a service principal using client certificate:

`az login --service-principal --username {{http://azure-cli-service-principal}} --password {{/path/to/cert.pem}} --tenant {{someone.onmicrosoft.com}}`

- Login using a VM's system assigned identity:

`az login --identity`

- Login using a VM's user assigned identity:

`az login --identity --username {{/subscriptions/subscription_id/resourcegroups/my_rg/providers/Microsoft.ManagedIdentity/userAssignedIdentities/my_id}}`