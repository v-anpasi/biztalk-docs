---
title: "IOneWayAsync.EndOneWayMethod Method | Microsoft Docs"
ms.custom: ""
ms.date: "06/08/2017"
ms.prod: "biztalk-server"
ms.reviewer: ""
ms.service: "biztalk-server"
ms.suite: ""
ms.tgt_pltfrm: ""
ms.topic: "article"
ms.assetid: 2d0b6f77-b4d6-4c0d-94a4-5c48081bf019
caps.latest.revision: 5
author: "MandiOhlinger"
ms.author: "mandia"
manager: "anneta"
---
# IOneWayAsync.EndOneWayMethod Method
\<End> method corresponding to **BeginTwoWayMethod** for the asynchronous operation implementation.  
  
> [!WARNING]
>  This topic is provided for information only. You can use this information to interpret the instances that WCF performance counters create for the WCF adapters and the auto-generated metadata for the WCF adapters. Do not rely on this information when you create applications.  
  
## Method Declaration  
  
```  
void EndTwoWayMethod(IAsyncResult result);  
```  
  
## Parameters  
 `result`  
 The status of the asynchronous operation.  
  
## See Also  
 [IOneWayAsync.BeginOneWayMethod Method](../core/ionewayasync-beginonewaymethod-method.md)