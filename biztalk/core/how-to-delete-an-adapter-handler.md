---
title: "How to Delete an Adapter Handler | Microsoft Docs"
ms.custom: ""
ms.date: "06/08/2017"
ms.prod: "biztalk-server"
ms.reviewer: ""
ms.service: "biztalk-server"
ms.suite: ""
ms.tgt_pltfrm: ""
ms.topic: "article"
helpviewer_keywords: 
  - "adapters, handlers"
  - "deleting, handlers [adapters]"
  - "handlers [adapters], deleting"
ms.assetid: 95db5652-e175-45d1-b713-1ad73655a592
caps.latest.revision: 11
author: "MandiOhlinger"
ms.author: "mandia"
manager: "anneta"
---
# How to Delete an Adapter Handler
You can delete a send or receive adapter handler by using the BizTalk Server Administration Console.  
  
 Before you remove an adapter handler, you must remove all receive locations or send ports with which it is associated.  
  
> [!NOTE]
>  You must be a member of the SSO Administration group to delete an adapter handler.  
  
### To delete an adapter handler  
  
1.  In the BizTalk Server Administration Console, expand **BizTalk Server Administration**, expand **BizTalk Group**, expand **Platform Settings**, and then expand **Adapters**.  
  
2.  In the expanded adapter list, select the adapter for which you want to delete the adapter handler.  
  
3.  Right-click the adapter handler that you want to delete, and then click **Delete**.  
  
4.  Click **Yes** to confirm that you want to delete this adapter handler.  
  
5.  Click **OK**.  
  
## See Also  
 [Creating and Deleting Adapter Handlers](../core/creating-and-deleting-adapter-handlers.md)