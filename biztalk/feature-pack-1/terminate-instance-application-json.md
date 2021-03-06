---
title: "Terminate instance application json | Microsoft Docs"
ms.custom: ""
ms.date: "06/08/2017"
ms.prod: "biztalk-server"
ms.reviewer: ""
ms.service: "biztalk-server"
ms.suite: ""
ms.tgt_pltfrm: ""
ms.topic: "managed-reference"
ms.assetid: 8ef43f1e-0c39-4812-84fc-aefc1b1b26c8
caps.latest.revision: 5
author: "tordgladnordahl"
ms.author: "tonordah"
manager: "anneta"
---
# Terminate instance: application/json
## Terminate instance

  Response Content Type: **application/json**

Request
---
Response Class (Status 200)

OK

Method  | Request URL
------------- | -------------
PUT  | http://biztalkfp1.westus.cloudapp.azure.com/BizTalkManagementService/OperationalData/Instances/Terminate/%7BinstanceId%7D

Response
---

| Response | Content          |
| ------------- | ----------- |
| Curl | curl -X PUT --header 'Accept: application/json' 'http://biztalkfp1.westus.cloudapp.azure.com/BizTalkManagementService/OperationalData/Instances/Terminate/%7BinstanceId%7D'|
| Response Code | 400|

Parameters
---

Parameter  | Value  | Description  | Parameter Type  | Data Type
------------- | ------------- | ------------- | ------------- | -------------
**instanceId** | | **instance Id** | path | string

Response Body
---
```
{
  "Message": "Please provide a valid instance Id"
}
```


Response Headers
---

```
{
  "pragma": "no-cache",
  "date": "Fri, 21 Apr 2017 03:23:06 GMT",
  "server": "Microsoft-IIS/10.0",
  "x-aspnet-version": "4.0.30319",
  "x-powered-by": "ASP.NET",
  "content-type": "application/json; charset=utf-8",
  "cache-control": "no-cache",
  "content-length": "48",
  "expires": "-1"
}
```

Example Value
---

```
{}

```
