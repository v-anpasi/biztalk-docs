---
title: "Configure the SOAP action for Siebel | Microsoft Docs"
ms.custom: ""
ms.date: "06/08/2017"
ms.prod: "biztalk-server"
ms.reviewer: ""
ms.service: "biztalk-server"
ms.suite: ""
ms.tgt_pltfrm: ""
ms.topic: "article"
helpviewer_keywords: 
  - "specifying SOAP action, at run time"
  - "specifying SOAP action, at design time"
  - "how to, specify SOAP action at design time"
  - "how to, specify SOAP action at run time"
ms.assetid: f22a4691-0355-4f08-a14e-e90a3c987ac0
caps.latest.revision: 9
author: "MandiOhlinger"
ms.author: "mandia"
manager: "anneta"
---
# Configure the SOAP action for Siebel
To perform any operation on the Siebel system using the WCF-based [!INCLUDE[adaptersiebel_short](../../includes/adaptersiebel-short-md.md)], adapter users must specify a SOAP action. The SOAP action communicates to the adapter what action should be performed. You can specify the SOAP action either at design time or at run time. However, if you specify the SOAP action both at design time and run time, the action you specified at design time will be overridden.  
  
 For more information about specifying SOAP action, see [Specifying SOAP Actions for WCF Send Adapters](../../core/specifying-soap-actions-for-wcf-send-adapters.md).
  
## Specifying SOAP Action at Design Time  
 For design time, you must specify the SOAP action as part of orchestration by including an expression shape.  
  
1.  In the BizTalk orchestration include an Expression shape by dragging it from the **BizTalk Orchestration** toolbox.  
  
2.  Double-click the **Expression** shape to open the BizTalk Expression Editor.  
  
3.  Specify the action in the BizTalk Expression Editor. For example:  
  
    ```  
    OutboundMessage(WCF.Action)="http://Microsoft.LobServices.Siebel/2007/03/BusinessObjects/Account/Account/Insert"  
    ```  
  
     For more information about **Expression** shape and the BizTalk Expression Editor, see [How to Create Expressions](../../core/how-to-create-expressions.md).  
  
## Specifying SOAP Action at Run Time  
 For run time, you must specify the SOAP action as part of the WCF-Custom or WCF-Siebel port properties dialog box.  
  
#### Enter a SOAP action for the WCF-Custom port  
  
1.  Start the [!INCLUDE[btsBizTalkServerNoVersion](../../includes/btsbiztalkservernoversion-md.md)] Administration console.  
  
2.  In the console tree, expand **BizTalk Group**, then expand **Applications**, and then click **Send Ports**. In the right pane, you can choose to create a port or select an existing port.  
  
3.  In the port properties dialog box, from the **Type** drop-down list, select **WCF-Custom**, and then click **Configure**.  
  
4.  In the **WCF-Custom Transport Properties** dialog box, click the **General** tab.  
  
5.  In the **Action** text box, specify the SOAP action for the operation. You can specify the action in the following ways:  
  
    -   **By using the single action format**. Use this format if the WCF-Custom port sends and receive messages for a single operation. For example:  
  
        ```  
        http://Microsoft.LobServices.Siebel/2007/03/BusinessObjects/Account/Account/Insert  
        ```  
  
    -   **By using the action mapping format**. Use this format if a single WCF-Custom port sends and receives messages for more than one operation. For example, if a single WCF-Custom port sends and receives messages for Op1 (to perform an Insert operation on Account business component) and Op2 (to perform an Update operation on Account business component), the SOAP action can be specified in the following manner:  
  
        ```  
        <BtsActionMapping>  
          <Operation Name="Op1" Action="http://Microsoft.LobServices.Siebel/2007/03/BusinessObjects/Account/Account/Insert " />  
          <Operation Name="Op2" Action="http://Microsoft.LobServices.Siebel/2007/03/BusinessObjects/Account/Account/Update " />  
        </BtsActionMapping>  
        ```  
  
         This approach provides greater flexibility in terms of specifying a set of actions and hence enabling messages belonging to different action types to flow through the same port.  
  
         The format for the SOAP action is different for each operation. For more information about action format for each operation, see the [Technical reference for the Siebel adapter](../../adapters-and-accelerators/adapter-siebel/technical-reference-for-the-siebel-adapter.md).  
  
#### Enter a SOAP action for the WCF-Siebel port  
  
1.  Start the [!INCLUDE[btsBizTalkServerNoVersion](../../includes/btsbiztalkservernoversion-md.md)] Administration console.  
  
2.  Add the WCF-Siebel adapter to the [!INCLUDE[btsBizTalkServerNoVersion](../../includes/btsbiztalkservernoversion-md.md)] Administration console. For instructions, see [Add the Siebel Adapter to BizTalk Server Administration Console](../../adapters-and-accelerators/adapter-siebel/add-the-siebel-adapter-to-biztalk-server-administration-console.md).  
  
3.  In the console tree, expand **BizTalk Group**, then expand **Applications**, and then click **Send Ports**. In the right pane, you can choose to create a port or select an existing port.  
  
4.  In the port properties dialog box, from the **Type** drop-down list, select the WCF-Siebel adapter you add earlier, and then click **Configure**.  
  
5.  In the port properties dialog box, click the **General** tab.  
  
6.  In the **Action** text box, specify the SOAP action for the operation. You can specify the action in the following ways:  
  
    -   **By using the single action format**. Use this format if the WCF-Custom port sends and receive messages for a single operation. For example:  
  
        ```  
        http://Microsoft.LobServices.Siebel/2007/03/BusinessObjects/Account/Account/Insert  
        ```  
  
    -   **By using the action mapping format**. Use this format if a single WCF-Custom port sends and receives messages for more than one operation. For example, if a single WCF-Custom port sends and receives messages for Op1 (to perform an Insert operation on Account business component) and Op2 (to perform an Update operation on Account business component), the SOAP action can be specified in the following manner:  
  
        ```  
        <BtsActionMapping>  
          <Operation Name="Op1" Action="http://Microsoft.LobServices.Siebel/2007/03/BusinessObjects/Account/Account/Insert " />  
          <Operation Name="Op2" Action="http://Microsoft.LobServices.Siebel/2007/03/BusinessObjects/Account/Account/Update " />  
        </BtsActionMapping>  
        ```  
  
         This approach provides greater flexibility in terms of specifying a set of actions and hence enabling messages belonging to different action types to flow through the same port.  
  
         The format for the SOAP action is different for each operation. For more information about action format for each operation, see the [Technical reference for the Siebel adapter](../../adapters-and-accelerators/adapter-siebel/technical-reference-for-the-siebel-adapter.md).  
  
## See Also  
[Building blocks to create BizTalk applications with the Siebel adapter](../../adapters-and-accelerators/adapter-siebel/building-blocks-to-create-biztalk-applications-with-the-siebel-adapter.md)