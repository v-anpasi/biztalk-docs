---
title: "Update Receive port application xml | Microsoft Docs"
ms.custom: ""
ms.date: "06/08/2017"
ms.prod: "biztalk-server"
ms.reviewer: ""
ms.service: "biztalk-server"
ms.suite: ""
ms.tgt_pltfrm: ""
ms.topic: "managed-reference"
ms.assetid: 5b123d4e-6f3f-4d0f-ac1e-39fdb5ce86a1
caps.latest.revision: 2
author: "tordgladnordahl"
ms.author: "tonordah"
manager: "anneta"
---
# Update Receive port: application/xml
## Update Receive Port


Parameters
---
|Parameter|Value|Description|Parameter Type|Data Type|
|---|---|---|---|---|
|receiveport|(required)|Receive port details|body|Example Value|

Example Value
---
```
\<?xml version="1.0"?>
<ReceivePort>
  <Name>string</Name>
  <Description>string</Description>
  <IsTwoWay>true</IsTwoWay>
  <ApplicationName>string</ApplicationName>
  <CustomData>string</CustomData>
  <InboundTransforms>string</InboundTransforms>
  <OutboundTransforms>string</OutboundTransforms>
  <Tracking>
    <Body>
      <BeforeSendPipeline>true</BeforeSendPipeline>
      <AfterSendPipeline>true</AfterSendPipeline>
      <BeforeReceivePipeline>true</BeforeReceivePipeline>
      <AfterReceivePipeline>true</AfterReceivePipeline>
    </Body>
    <Property>
      <BeforeSendPipeline>true</BeforeSendPipeline>
      <AfterSendPipeline>true</AfterSendPipeline>
      <BeforeReceivePipeline>true</BeforeReceivePipeline>
      <AfterReceivePipeline>true</AfterReceivePipeline>
    </Property>
  </Tracking>
  <ReceiveLocations>string</ReceiveLocations>
  <PrimaryReceiveLocation>string</PrimaryReceiveLocation>
</ReceivePort>

```


Response Messages
---
|HTTP Status Code|Reason|Response Model|Headers|
|---|---|---|---|
|204|No Content|||



