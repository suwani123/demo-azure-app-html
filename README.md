# demo-azure-app-html

---
topic: HTML Hello World
languages:
  - HTML
products:
  - Azure App Service
  - Azure Web Apps
---

# HTML Hello World

This sample demonstrates a tiny Hello World HTML app for [App Service](https://docs.microsoft.com/azure/app-service).

# App service (demo-azure-app-html) deply via CLI command
- Login to Azure Portal
- Open azure bash environment
- Create a folder 
---
mkdir htmlapp
cd htmlapp
--
- Clone the app from the repository
git clone https://github.com/suwani123/demo-azure-app-html.git
- change the project folder
cd demo-azure-app-html
-- Create the azure app service 
    az webapp up --location <myLocation> --name <myAppName> --html
    (e.g. az webapp up --location eastasia --name demoapphtml --html)
- Refer the below command to clean up resources
  az group delete --name <resource_group> --no-wait
  
# Contributing

This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/). For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.
