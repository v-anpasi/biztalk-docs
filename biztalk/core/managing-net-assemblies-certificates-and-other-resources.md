---
title: "Managing .NET Assemblies, Certificates, and Other Resources | Microsoft Docs"
ms.custom: ""
ms.date: "06/08/2017"
ms.prod: "biztalk-server"
ms.reviewer: ""
ms.service: "biztalk-server"
ms.suite: ""
ms.tgt_pltfrm: ""
ms.topic: "article"
helpviewer_keywords: 
  - "managing [certificates], about managing certificates"
  - ".NET assemblies, managing"
  - "managing [.NET assemblies]"
  - "managing [resources], .NET assemblies"
  - "managing [resources], certificates"
  - "managing [certificates]"
  - "managing [.NET assemblies], about managing .NET assemblies"
  - "certificates, managing"
ms.assetid: efe27a11-19d8-4eb3-9f8c-f4336e4c3d66
caps.latest.revision: 13
author: "MandiOhlinger"
ms.author: "mandia"
manager: "anneta"
---
# Managing .NET Assemblies, Certificates, and Other Resources
This section provides instructions on using the BizTalk Server Administration console and the BTSTask command-line tool to manage the following types of resource artifacts for a BizTalk application. These resource artifacts cannot be automatically deployed into a BizTalk application from Visual Studio, so you must add them manually to the application. Once added to an application, however, you can import, export, and install them as a unit with the application and its other artifacts.  
  
-   **Files.** You can include ad hoc files, such as a Readme file. When you install the application, files are copied to the installation folder.  
  
-   **Certificates.** You can add a certificate file to an application so that you can transport the certificate from one BizTalk group to another, packaged with an application. You assign certificates to send ports and receive locations to verify identities and to establish secure links.  
  
-   **COM and COM+ components.** You can include managed COM and managed COM+ components to provide additional functionality in a BizTalk application.  
  
-   **.NET assemblies.** You can include .NET assemblies that are not specifically BizTalk assemblies in a BizTalk application. (BizTalk assemblies are .NET assemblies that contain BizTalk orchestrations, pipelines, schemas, or maps.)  
  
-   **BAM definition files.** To make BAM deployment easier, you can create a BizTalk application and add BAM definitions to it. You can then use the BizTalk application deployment features to deploy the BAM definitions into different environments.  
  
-   **Binding files.** You can add binding files to an application to make moving an application from one deployment environment to another quicker and easier.  
  
-   **Virtual directories.** You can add virtual directories to your application so that they will be deployed with the application.  
  
> [!NOTE]
>  You can use Microsoft Windows Management Instrumentation (WMI) Object Model to create and run scripts that automate administrative tasks. For information about using WMI, see [WMI Class Reference](../core/wmi-class-reference.md).  
  
## In This Section  
  
-   [How to Add a File to an Application](../core/how-to-add-a-file-to-an-application.md)  
  
-   [How to Add a Certificate to an Application](../core/how-to-add-a-certificate-to-an-application.md)  
  
-   [How to Add a COM Component to an Application](../core/how-to-add-a-com-component-to-an-application.md)  
  
-   [How to Add a .NET Assembly to an Application](../core/how-to-add-a-net-assembly-to-an-application.md)  
  
-   [How to Add a BAM Artifact to an Application](../core/how-to-add-a-bam-artifact-to-an-application.md)  
  
-   [How to Add a Binding File to an Application](../core/how-to-add-a-binding-file-to-an-application2.md)  
  
-   [How to Add a Virtual Directory to an Application](../core/how-to-add-a-virtual-directory-to-an-application.md)  
  
-   [How to Modify the Deployment Options of a .NET Assembly, COM Component, File, or BAM Artifact](../core/modify-deployment-options-of-net-assembly-com-component-file-bam-artifact.md)  
  
-   [How to Remove a .NET Assembly, Certificate, or Other Resource Artifact from an Application](../core/remove-a-net-assembly-certificate-or-resource-artifact-from-an-application.md)