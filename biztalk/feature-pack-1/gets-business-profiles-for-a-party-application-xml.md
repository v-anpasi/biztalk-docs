---
title: "Gets business profiles for a Party application xml | Microsoft Docs"
ms.custom: ""
ms.date: "06/08/2017"
ms.prod: "biztalk-server"
ms.reviewer: ""
ms.service: "biztalk-server"
ms.suite: ""
ms.tgt_pltfrm: ""
ms.topic: "managed-reference"
ms.assetid: f368bd23-063e-4e6c-b435-99547c64bb88
caps.latest.revision: 3
author: "tordgladnordahl"
ms.author: "tonordah"
manager: "anneta"
---
# Gets business profiles for a Party: application/xml
## Gets business profiles for a Party

  Response Content Type: **application/xml**

Request
---
Response Class (Status 200)

OK

Parameters
---


Parameter|Value|Description|Parameter Type|Data Type  
---------|---------|---------|---------|---------
partyName|(required)|Party name|path|string|

Example Value
---

```
\<?xml version="1.0"?>
<Inline Model>
  <Name>string</Name>
  <Description>string</Description>
  <BusinessIdentities>
    <Description>string</Description>
    <Qualifier>string</Qualifier>
    <Value>string</Value>
    <Id>1</Id>
  </BusinessIdentities>
  <CustomSettings>
    <Name>string</Name>
    <Value>string</Value>
  </CustomSettings>
\</Inline Model>
```