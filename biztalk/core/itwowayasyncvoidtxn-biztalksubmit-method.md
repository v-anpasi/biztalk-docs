---
title: "ITwoWayAsyncVoidTxn.BizTalkSubmit Method | Microsoft Docs"
ms.custom: ""
ms.date: "06/08/2017"
ms.prod: "biztalk-server"
ms.reviewer: ""
ms.service: "biztalk-server"
ms.suite: ""
ms.tgt_pltfrm: ""
ms.topic: "article"
ms.assetid: 3be75cd9-a235-478a-922c-dfcc287dc6b1
caps.latest.revision: 5
author: "MandiOhlinger"
ms.author: "mandia"
manager: "anneta"
---
# ITwoWayAsyncVoidTxn.BizTalkSubmit Method
Causes the runtime to create WSDL operations in the metadata. This method should never get invoked.  
  
> [!WARNING]
>  This topic is provided for information only. You can use this information to interpret the instances that WCF performance counters create for the WCF adapters and the auto-generated metadata for the WCF adapters. Do not rely on this information when you create applications.  
  
## Method Declaration  
  
```  
[OperationContract(IsOneWay = false, Action = "BizTalkSubmit")]  
[TransactionFlow(TransactionFlowOption.Mandatory)]  
Message BizTalkSubmit(Message message);  
```  
  
## Return Value  
 This method throws the **NotSupportedException** if called.  
  
## See Also  
 [NotSupportedException Class](http://go.microsoft.com/fwlink/?LinkId=88629)