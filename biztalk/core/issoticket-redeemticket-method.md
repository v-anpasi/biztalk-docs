---
title: "ISSOTicket.RedeemTicket Method | Microsoft Docs"
ms.custom: ""
ms.date: "06/08/2017"
ms.prod: "biztalk-server"
ms.reviewer: ""
ms.service: "biztalk-server"
ms.suite: ""
ms.tgt_pltfrm: ""
ms.topic: "article"
ms.assetid: ad89b448-0064-4158-bcc0-73ef93be9993
caps.latest.revision: 5
author: "MandiOhlinger"
ms.author: "mandia"
manager: "anneta"
---
# ISSOTicket.RedeemTicket Method
The **RedeemTicket** method redeems an Enterprise Single Sign-On (SSO) server ticket that was previously issued with the **IssueTicket** method.  
  
## Syntax  
  
```cpp#  
  
HRESULT RedeemTicket(  
BSTR bstrApplicationName,  
BSTR bstrTicket,  
LONG lFlags,  
BSTR* pbstrExternalUserName,  
SAFEARRAY BSTR  
);  
```  
  
#### Parameters  
 `bstrApplicationName`  
 [in]  String that specifies the application name. This parameter cannot be NULL, an empty string, or contain spaces. Application names are not case-sensitive, but case will be preserved. For example, ABC, abc, and AbC are considered to be the same application.  
  
 `bstrTicket`  
 [in]  String that specifies the ticket value obtained from the **IssueTicket** method.  
  
 `lFlags`  
 [in]  Long integer that specifies the flags to set. Use the flag SSO_FLAG_REFRESH to indicate that the credential cache should be bypassed.  
  
 `pbstrExternalUserName`  
 [out]  Pointer to a string that receives the external user name associated with the ticket.  
  
 `BSTR`  
 [out]  String that receives the external credentials associated with the ticket. If there are no credentials, the size of the returned array is zero.  
  
## Return Value  
 This method returns an HRESULT indicating whether it completed successfully. For more details, see the Error Values section.  
  
## Error Values  
 This method returns an HRESULT containing one of the values in the following table.  
  
|Value|Description|  
|-----------|-----------------|  
|S_OK|The method succeeded.|  
|E_ACCESSDENIED|Access is denied to the caller.|  
|E_INVALIDARG|An invalid parameter was detected.|  
  
## Remarks  
 Because the credentials are returned in plain text by this method, the caller should be careful to clear (overwrite) them as soon as possible after use.  
  
 To access this method, you must be an SSO Administrator, SSO Affiliate Administrator, or an Application Administrator.  
  
## Requirements  
 **Platforms:**  [!INCLUDE[btsPlatformsComApis](../includes/btsplatformscomapis-md.md)]  
  
## See Also  
 [ISSOTicket Interface (COM)](../core/issoticket-interface-com.md)   
 [ISSOTicket Members](../core/issoticket-members.md)   
 [Programming with Enterprise Single Sign-On](../core/programming-with-enterprise-single-sign-on.md)