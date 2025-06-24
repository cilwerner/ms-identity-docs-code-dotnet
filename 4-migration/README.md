---
page_type: sample
languages:
- csharp
products:
- azure-active-directory
- dotnet
description: "Guidance to help migrate web applications from AD FS to Azure AD"
urlFragment: "ms-identity-dotnet-adfs-to-aad"
---

# AD FS to Azure AD application migration playbook for developers

This set of ASP.NET code samples and accompanying tutorials will help you learn how to safely and securely migrate your applications integrated with Active Directory Federation Services (AD FS) to Azure Active Directory (Azure AD). This tutorial is focused towards developers who not only need to learn configuring apps on both AD FS and Azure AD, but also become aware and confident of changes their code base will require in this process.

These code samples are a companion to [Moving application authentication from AD FS to Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/migrate-adfs-apps-to-azure) available on the Microsoft Docs site.   

The folders in this repo are arranged as *chapters*, each with a README and sample code for a scenario. The chapters cover the most common types of authentication utilized by applications integrated with AD FS today, and we hope they let you learn and gain valuable experience before undertaking an app migration initiative for your applications currently running in production.

## Prerequisites

- [.NET Framework 4.7.2](https://dotnet.microsoft.com/download/dotnet-framework)
- [AD FS](https://docs.microsoft.com/windows-server/identity/ad-fs/ad-fs-overview) environment
- [Azure AD tenant](https://docs.microsoft.com/azure/active-directory/develop/quickstart-create-new-tenant)

## Migration steps

By following the tutorial chapters in this code sample, you progress through the following scenarios:

- We start by integrating the provided sample web application with an AD FS instance. This web app uses the [SAML](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol) protocol for it authentication setup. 
- Next, we'd migrate this application to an Azure AD tenant.
- Finally, we also provide instructions as how to change the authentication protocol from SAML to [OAuth 2.0 and OpenID Connect](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-protocols). This change allows you to reap the benefits of accessing rich APIs like [Microsoft Graph](https://docs.microsoft.com/graph/overview) and the [Azure REST API](https://docs.microsoft.com/rest/api/azure/) amongst others.

We have also covered the following topics in some detail as they might play a big part in your app migration work:

- Configuring [Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-whatis).
- Migrating [Directory Extensions](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-feature-directory-extensions) to Azure AD.
- Sync and use Security Groups on the migrated application.

## Contents

### Chapter 1: Integrate sample app with AD FS

|                                                  |                               |
|--------------------------------------------------|-------------------------------|
| [1.1 Integrate app with AD FS](1-ADFS-Host/1-1-Setup-SAML-Playground/README.md) | Integrate the provided ASP.NET MVC web application with an AD FS instance. |
| [1.2 Set up Azure AD Connect](1-ADFS-Host/1-2-Setup-AzureADConnect/README.md) | A brief look at the Azure AD Connect configuration that synchronizes on=premise data to an Azure AD tenant. |
| [1.3 Directory Extensions](1-ADFS-Host/1-3-Directory-Extensions/README.md) | Migrate Directory Extensions from on-prem Active Directory to your Azure AD tenant .|

### Chapter 2: Migrate the working web app from AD FS to Azure AD

|                                                  |                               |
|--------------------------------------------------|-------------------------------|
| [2.1 Integrate app with Azure AD](2-AAD-Migration/2-1-SAML-WebApp/README.md)| Migrating the SAML ASP.NET MVC web app from AD FS to Azure AD.|
| [2.2 Using Security groups](2-AAD-Migration/2-2-Security-Groups/README.md) | Using on-premise Active Directory security groups in applications migrated to an Azure AD tenant. |
| [2.3 Convert from SAML to OIDC](2-AAD-Migration/2-3-From-SAML-to-OIDC/README.md) | Migrate a SAML ASP.NET application to use [OAuth 2.0 and OpenID Connect](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-protocols).|

For information about Integrated Windows Authentication (IWA), see [Azure-Samples/active-directory-dotnet-iwa-v2](https://github.com/Azure-Samples/active-directory-dotnet-iwa-v2).

## We'd love your feedback!

Were we successful in addressing your learning objective? [Do consider taking a moment to share your experience with us.](https://forms.office.com/Pages/ResponsePage.aspx?id=v4j5cvGGr0GRqy180BHbR73pcsbpbxNJuZCMKN0lURpUODFCRVg4VTk2QUE2VEFPMUZKSEJNUFhWUyQlQCN0PWcu)

We're always listening, and if you want to get in touch with you directly, send an email to <aadappfeedback@microsoft.com>.


## Community Help and Support

Use [Stack Overflow](http://stackoverflow.com/questions/tagged/msal) to get support from the community.

If you find a bug in the sample, raise the issue on [GitHub Issues](../issues).

To provide feedback on or suggest features for Azure Active Directory, visit [User Voice](https://feedback.azure.com/forums/169401-azure-active-directory).

## Contributing

This project welcomes contributions and suggestions.  Most contributions require you to agree to a
Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us
the rights to use your contribution. For details, visit https://cla.opensource.microsoft.com.

When you submit a pull request, a CLA bot will automatically determine whether you need to provide
a CLA and decorate the PR appropriately (e.g., status check, comment). Simply follow the instructions
provided by the bot. You will only need to do this once across all repos using our CLA.

This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/).
For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or
contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.
