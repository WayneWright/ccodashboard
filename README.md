
# Continuous Cloud Optimization Power BI Dashboard

## Content

- [Overview](README.md#overview)
- [List of resources](README.md#List-of-resources)
- [CCO Dashboard report pages](README.md#CCO-Dashboard-report-Pages)
- [CCO Dashboard AKS add-on report pages](README.md#CCO-Dashboard-AKS-add-on)
- [Call for Contribution](README.md#Call-for-Contribution)
-------------------------------


## Overview
The Continuous Cloud Optimization Power BI Dashboard (referred as CCO Dashboard here after) is a Power BI Dashboard developed using Power Query M language that pulls information directly from different Azure and Graph REST APIs. It presents the information in a simplified format to track potential recommendations from Azure Advisor or Azure Security Center allowing you to filter by subscriptions, resources groups, tags or particular resources.

![OverviewImage](/install/images/OverviewImage.png)

## List of resources
This project includes the following resources:

1. **install folder**: Includes all the files required to successfully deploy the Dashboard in your environment. The [Deployment Guide](/install/DeploymentGuide.md) file contains a detailed guidance to install and setup your dashboard including the requirements, what REST APIs are in use, the resource providers that needs to be enabled or what tabs are included as part of the default Dashboard. The [Troubleshooting Guide](/install/TroubleshootingGuide.md) file contains guidance to solve potential issues that you might encounter during the Dashboard deployment. Errors like Power BI regional settings, or Privacy levels will be documented on this document.
2. **queries folder**: Includes the M queries used in the Dashboard to pull data from Azure and Graph REST APIs. This content is for reference purposes to facilitate the Data Model comprehension and to enable contributors to expand the Dashboard capabilities. 
3. **docs/assets/pictures folder**: Contains all the images that the Dashboard will use when loading data from Azure. The content of this folder will be dynamic and we will update the repository regularly. Make sure the computer running the Dashboard that has internet access also have access to this URL https://azure.github.io/ccodashboard/assets/pictures
4. **dashboards folder**: This parent folder contains sub folders with different versions of the CCO Dashboard depending on the workloads you want to get report from. We expect to see more versions in the future from community contributions.
    - ***CCODashboard folder*** has a more generic version of the Dashboard that includes information from Azure Advisor, Azure Security Center, Azure Networking REST APIs, Azure Compute REST APIs and Graph
    - ***CCODashboard-AKS folder*** has the add-on report to monitor Azure Kubernetes Services.

## CCO Dashboard report pages
The version 4.0 of the CCO Power BI Dashboard includes 7 report pages. You will be able to navigate, filter and report the following information:
- Page 1: Overview
- Page 2: Azure Advisor Recommendations
- Page 3: Azure Security Center Task recommendations
- Page 4: Azure Security Center Alerts
- Page 5: Azure Networking information
- Page 6: Azure Compute information
- Page 7: Azure RBAC permissions
  
You can find more details about each page on the [Deployment Guide](/install/DeploymentGuide.md) file

## CCO Dashboard AKS add-on report pages

The version 4.0 of the CCO Power BI Dashboard AKS add-on includes the following information

- Azure Kubernetes Clusters
- Azure Container Images running on AKS Clusters
- Azure Container Registries
- Nodes, Pods, Containers status from Azure Log Analytics

## Call for contribution
This project welcomes contributions and suggestions.  Most contributions require you to agree to a
Contributor License Agreement (CLA) declaring that you have the right to, and actually do grant us
the rights to use your contribution. For details, visit https://cla.microsoft.com.

When you submit a pull request, a CLA-bot will automatically determine whether you need to provide
a CLA and decorate the PR appropriately (e.g., label, comment). Simply follow the instructions
provided by the bot. You will only need to do this once across all repos using our CLA.

This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/).
For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or
contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.
