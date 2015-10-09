---
services: billing
platforms: dotnet
author: bryanla
---

# Microsoft Azure Billing API Code Samples: Multi-Tenant Web Application 
A Web application that allows the signed-in user to give consent to the application, to call the Azure Graph API and the Azure Usage API on the user's behalf. It also shows the OAuth flows required to get consent for the ‘Reader’ role, for the list of Microsoft Azure subscriptions that the user wants to allow access to. The Microsoft Azure Billing APIs enable integration of Azure Billing information into your applications, providing new insights into your consumption of Azure resources, allowing you to accurately predict and manage your Azure resource consumption costs.  

The application first lists all subscriptions that the signed-in user has access to, and then lets the user choose which subscription to use for pulling Usage data. After the subscription is selected, the app retrieves and deserializes the Usage response data, and displays it on the page. 

This sample also demonstrates the Multi-Tenant functionality in Azure Active Directory (AAD), which is required in partner/ISV scenarios where you are building a Web App that requires sign-in and consent from multiple AAD tenants, to grant access to their directories. 

To learn more about the Billing Usage and RateCard APIs, visit the overview article [Gain insights into your Microsoft Azure resource consumption](https://azure.microsoft.com/documentation/articles/billing-usage-rate-card-overview/).  Visit the [Azure Billing REST API Reference](https://msdn.microsoft.com/en-us/library/azure/mt218998.aspx) article for more details on each of the APIs.

## Get started

First, download the source code using your favorite **git** shell or command line (ie: Git Bash, Git for Windows, etc.). For example, if you're using Git Bash:

    git clone https://github.com/Azure-Samples/billing-dotnet-webapp-multitenant.git
    cd billing-dotnet-webapp-multitenant

Then follow the steps in [the solution readme](./WebApp-Billing-MultiTenant) to complete the required configuration work and build the sample in Visual Studio.

## Complete billing samples index
Below is the list of all of the available Azure Billing API code samples:

-	[billing-dotnet-usage-api](https://github.com/Azure-Samples/billing-dotnet-usage-api) - This sample will help you get started with the Usage API.
-	[billing-dotnet-ratecard-api](https://github.com/Azure-Samples/billing-dotnet-ratecard-api/) - This sample help you get started with the RateCard API.
-	[billing-dotnet-webapp-multitenant](https://github.com/Azure-Samples/billing-dotnet-webapp-multitenant/) - This Multi-Tenant sample creates a WebApp that allows the signed-in user to give it consent, to call the Azure Graph API and the Usage API on the user's behalf. It also shows the OAuth flows required to get consent for the ‘Reader’ role, to access the list of Microsoft Azure subscriptions that the user wants to allow access to. 

## Need Help?

Be sure to check out the Azure forums on [StackOverflow](http://stackoverflow.com/search?q=azure+billing) and [MSDN](https://social.msdn.microsoft.com/Forums/azure/en-US/home?forum=windowsazurepurchasing) if you are having trouble. The Azure Billing product team actively monitors the forums and will be more than happy to assist you.

If you would like to provide feedback on the Billing APIs or ideas on how we can improve them, please visit the [Azure Feedback Forums](http://feedback.azure.com/forums/170030-billing).

## Contribute Code or Provide Feedback

If you would like to become an active contributor to this project please follow the instructions provided in [Microsoft Azure Projects Contribution Guidelines](http://azure.github.com/guidelines.html).

If you encounter any bugs with the library please file an issue in the [Issues](https://github.com/Azure-Samples/billing-dotnet-webapp-multitenant/issues) section of the repository.

## Learn More
* [Azure Billing REST API Reference ](https://msdn.microsoft.com/library/azure/1ea5b323-54bb-423d-916f-190de96c6a3c)
