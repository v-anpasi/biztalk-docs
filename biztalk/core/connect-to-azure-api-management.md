---
title: "Connect to Azure API Management | Microsoft Docs"
ms.custom: ""
ms.date: "06/08/2017"
ms.reviewer: ""
ms.suite: ""
ms.tgt_pltfrm: ""
ms.topic: "article"
ms.assetid: a87bfb40-7e6f-46aa-8ac7-db6d13ce7eb2
caps.latest.revision: 2
author: "tordgladnordahl"
ms.author: "tonordah"
manager: "anneta"
---
# Connect to Azure API Management
You can now easily expose your SOAP endpoint through API Management from BizTalk.

## What is Azure API Management
Use Azure API Management as a turnkey solution for publishing APIs to external and internal customers. Quickly create consistent and modern API gateways for existing back-end services hosted anywhere, secure and protect them from abuse and overuse, and get insights into usage and health. Plus, automate and scale developer onboarding to help get your API program up and running. 
[Click here](https://azure.microsoft.com/en-us/services/api-management/) to learn more about API Management

## Prerequisites
* Configure and set up [Azure API Management](https://docs.microsoft.com/en-us/azure/api-management/api-management-get-started)
* Create a [virtual network](https://docs.microsoft.com/en-us/azure/api-management/api-management-using-with-vnet) between your BizTalk Machine and the API Managemenet instance


1. In the Azure Portal open up your API managmenet and select **APIs** From the menu

	![select API for BizTalk](../core/media/select-api-for-biztalk.png)
	
2. Select the option for **WSDL** in the New API section

	![select wsdl biztalk api](../core/media/select-wsdl-biztalk-api.png)
	
3. To connect to API Management to your BizTalk WSDL copy the URL to your BizTalk Machine with the full URI to your SOAP endpoint eg. `http://10.0.31.22/RestEndPoint/OrderIncome.svc?wsdl`

	![create API from WSDL BizTalk](../core/media/create-api-from-wsdl-biztalk.png)

4. Select if you want to to a **SOAP pass-through** or set up a **SOAP to REST** service
5. Fill in the **name** of your API as well as **Description** and the **API Url suffix** for your service
6. Click **Create** to establish the communication to your backend SOAP endpoint
7. 