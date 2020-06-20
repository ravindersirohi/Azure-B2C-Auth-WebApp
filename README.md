# Azure-B2C-Auth-WebApp
.Net Core Web App Authentication with Azure B2C along with public identity provider like google.

# Azure B2C Configuraitons
1) To create a Azure B2C Tenant - https://docs.microsoft.com/en-gb/azure/active-directory-b2c/tutorial-create-tenant <br/>
2) To configure External identity provider - https://docs.microsoft.com/en-us/azure/active-directory-b2c/identity-provider-google <br/>
3) To register web app in Azure B2C - https://docs.microsoft.com/en-gb/azure/active-directory-b2c/tutorial-register-applications?tabs=app-reg-ga#register-a-web-application

# Web App Configurations

{
  "AzureAdB2C": {
    "Instance": "https://<your-tenant-name>.b2clogin.com",
    "ClientId": "<web-app-application-id>",
    "Domain": "<your-b2c-domain>",
    "SignedOutCallbackPath": "/signout/<your-sign-up-in-policy>",
    "SignUpSignInPolicyId": "<your-sign-up-in-policy>"
  }
}
