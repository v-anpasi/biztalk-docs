---
title: "Create Receive Port application x www form urlencoded | Microsoft Docs"
ms.custom: ""
ms.date: "06/08/2017"
ms.prod: "biztalk-server"
ms.reviewer: ""
ms.service: "biztalk-server"
ms.suite: ""
ms.tgt_pltfrm: ""
ms.topic: "managed-reference"
ms.assetid: 8fc664b3-e592-4dab-9163-75a5dc67bfee
caps.latest.revision: 2
author: "tordgladnordahl"
ms.author: "tonordah"
manager: "anneta"
---
# Create Receive Port: application/x-www-form-urlencoded
## Create Receive Port


Parameters
---
|Parameter|Value|Description|Parameter Type|Data Type|
|---|---|---|---|---|
|receiveport|(required)|Receive port details|body|Example Value|

Example Value
---
```
{
  "Name": "string",
  "Description": "string",
  "IsTwoWay": true,
  "ApplicationName": "string",
  "CustomData": "string",
  "InboundTransforms": [
    "string"
  ],
  "OutboundTransforms": [
    "string"
  ],
  "Tracking": {
    "Body": {
      "BeforeSendPipeline": true,
      "AfterSendPipeline": true,
      "BeforeReceivePipeline": true,
      "AfterReceivePipeline": true
    },
    "Property": {
      "BeforeSendPipeline": true,
      "AfterSendPipeline": true,
      "BeforeReceivePipeline": true,
      "AfterReceivePipeline": true
    }
  },
  "ReceiveLocations": [
    "string"
  ],
  "PrimaryReceiveLocation": "string"
}
```


Response Messages
---
|HTTP Status Code|Reason|Response Model|Headers|
|---|---|---|---|
|204|No Content|||



