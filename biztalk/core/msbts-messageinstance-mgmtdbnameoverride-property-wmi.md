---
title: "MSBTS_MessageInstance.MgmtDbNameOverride Property (WMI) | Microsoft Docs"
ms.custom: ""
ms.date: "06/08/2017"
ms.prod: "biztalk-server"
ms.reviewer: ""
ms.service: "biztalk-server"
ms.suite: ""
ms.tgt_pltfrm: ""
ms.topic: "article"
ms.assetid: 872af0b8-43c1-45ec-b092-4a1366c730f2
caps.latest.revision: 8
author: "MandiOhlinger"
ms.author: "mandia"
manager: "anneta"
---
# MSBTS_MessageInstance.MgmtDbNameOverride Property (WMI)
Overrides the initial catalog part of the BizTalk Management database connect string, and represents the database name. This property was not implemented for [!INCLUDE[btsBizTalkServer2006r3](../includes/btsbiztalkserver2006r3-md.md)] and is reserved for future use.  
  
 *The syntax shown is language neutral.*  
  
## Syntax  
  
```  
  
string MgmtDbNameOverride = "";  
```  
  
## Remarks  
 This property is optional.  
  
 This property is read-only.  
  
 This property has a **Key** qualifier. Along with **MessageInstanceID**, **MgmtDbServerOverride**, and **ServiceInstanceID**, this key forms a compound key for the class.  
  
 The maximum length for this property is 123 characters.  
  
## Requirements  
 **Header:** Declared in BTSWMISchemaXP.mof.  
  
 **Namespace:** Included in \root\MicrosoftBizTalkServer.