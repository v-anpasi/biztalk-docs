---
title: "Add a party alias application json | Microsoft Docs"
ms.custom: ""
ms.date: "06/08/2017"
ms.prod: "biztalk-server"
ms.reviewer: ""
ms.service: "biztalk-server"
ms.suite: ""
ms.tgt_pltfrm: ""
ms.topic: "managed-reference"
ms.assetid: feadee2e-4912-4cc5-8d32-f3d221056b30
caps.latest.revision: 3
author: "tordgladnordahl"
ms.author: "tonordah"
manager: "anneta"
---
# Add a party alias: application/json
## Add a party alias

  Response Content Type: **application/json**


Method  | Request URL
------------- | -------------
POST  | http://biztalkfp1.westus.cloudapp.azure.com/BizTalkManagementService/Parties/%7BpartyName%7D

Response
---

| Response | Content          |
| ------------- | ----------- |
| Curl | curl -X POST --header 'Content-Type: application/json' --header 'Accept: application/json' -d '{partyName}' 'http://biztalkfp1.westus.cloudapp.azure.com/BizTalkManagementService/Parties/%7BpartyName%7D'|
| Response Code | 404|


Response Body
---
```
{
  "Message": "Party {partyName} does not exist."
}
```

Response Headers
---

```
{
  "pragma": "no-cache",
  "date": "Tue, 25 Apr 2017 00:57:54 GMT",
  "server": "Microsoft-IIS/10.0",
  "x-aspnet-version": "4.0.30319",
  "x-powered-by": "ASP.NET",
  "content-type": "application/json; charset=utf-8",
  "cache-control": "no-cache",
  "content-length": "47",
  "expires": "-1"
}
```

Parameters
---
Parameter  | Value  | Description  | Parameter Type  | Data Type
------------- | ------------- | ------------- | ------------- | -------------
| **partyAlias** | | **Party Alias details** | body | Example Value
| **partyName**  | | **Party Name** | path | string

Example Value
---
```
{
  "Name": "string",
  "Qualifier": "string",
  "Value": "string",
  "IsAutoCreated": true
}
```
Response Messages
---

HTTP Status Code  | Reason  | Response Model  | Headers
------------- | ------------- | ------------- | -------------
204 | No Content|  |  | 

