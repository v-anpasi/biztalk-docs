---
title: "Glossary9 | Microsoft Docs"
ms.custom: ""
ms.date: "06/08/2017"
ms.prod: "biztalk-server"
ms.reviewer: ""
ms.service: "biztalk-server"
ms.suite: ""
ms.tgt_pltfrm: ""
ms.topic: "article"
helpviewer_keywords: 
  - "glossary"
ms.assetid: 75c74760-53b6-45c3-bacc-bb7ab4fb5b4b
caps.latest.revision: 3
author: "MandiOhlinger"
ms.author: "mandia"
manager: "anneta"
---
# Glossary
The following terms and definitions are used in [!INCLUDE[adaptersiebel](../../includes/adaptersiebel-md.md)] Help.  
  
## Microsoft BizTalk Adapter Pack Glossary  
 [A](#A) [B](#B) [C](#C) [D](#D) [E](#E) F [G](#G)[H](#H)[I](#I) J K L [M](#M) N [O](#O)[P](#P) Q [R](#R)[S](#S) T [U](#U) V [W](#W)[X](#X) Y Z  
  
####  <a name="A"></a> A  
  
|||  
|-|-|  
|adapter|A WCF-based component that helps exchange messages between applications (for example, a line-of-business system) and BizTalk Server. The adapter consists of design-time components and run-time components for receive and send operations.|  
|adapter client|Refers to an application that is interacting with a line-of-business (LOB) system through the adapter.|  
  
####  <a name="B"></a> B  
  
|||  
|-|-|  
|binding|A process by which software components and layers are linked together. When a network component is installed, the binding relationships and dependencies for the components are established. Binding allows components to communicate with each other. In BizTalk Server, an established mapping between an orchestration adapter-agnostic endpoint (port or role link) and physical adapter-specific endpoints (send/receive ports or party).|  
|BizTalk Server|Connects diverse software. BizTalk Server enables you to create and modify process logic that uses that software. BizTalk Server also enables information workers to monitor running processes, interact with trading partners, and perform other business-oriented tasks.|  
  
####  <a name="C"></a> C  
  
|||  
|-|-|  
|channel|A concrete implementation of a binding element. The binding represents the configuration, and the channel is the implementation associated with that configuration. Therefore, there is a channel associated with each binding element. Channels stack on top of each other to create the concrete implementation of the binding: the channel stack.|  
|connection URI|A string that identifies a resource in a distributed environment. Adapters use a connection Uniform Resource Indicator (URI) that contains the information necessary to establish a connection with the LOB system.|  
|contract|Specifies the collection and structure of messages required to access the operations offered by the service.|  
  
####  <a name="D"></a> D  
  
|||  
|-|-|  
|design-time experience|Procedures and operations that a developer performs during design time; for example, using the Consume Adapter Service BizTalk Project Add-in to retrieve message schemas.|  
  
####  <a name="E"></a> E  
  
|||  
|-|-|  
|endpoint address|A network address that identifies the location of a Windows Communication Foundation (WCF) service endpoint. For an adapter, the endpoint address is expressed as a connection Uniform Resource Identifier (URI) that contains location and connection parameters. The adapter can use these to establish a connection to the underlying line-of-business (LOB) system.|  
|Enterprise Single Sign-on system|An SSO database, a master secret server, and one or more Enterprise Single Sign-On (SSO) servers. These servers do the mapping between the Windows and non-Windows credentials, look up the credentials in the SSO database, and are used for administering the SSO system. The SSO database is also used as a configuration store to hold custom configuration data for adapters.|  
|Extensible Markup Language|A markup language designed to describe data. XML tags are not predefined.|  
  
####  <a name="G"></a> G  
  
|||  
|-|-|  
|GAC|See global assembly cache.|  
|global assembly cache (GAC)|A machine-wide code cache that stores assemblies specifically installed to be shared by many applications on the computer. Applications deployed in the global assembly cache must have a strong name.|  
  
####  <a name="H"></a> H  
  
|||  
|-|-|  
|Health and Activity Tracking (HAT)|A user interface that enables specified data to be tracked. This interface can be used to monitor the health of the BizTalk server farm and to track and view specific events and messages.|  
  
####  <a name="I"></a> I  
  
|||  
|-|-|  
|inbound operation|An operation that is invoked by a line-of-business (LOB) system on the adapter.|  
  
####  <a name="M"></a> M  
  
|||  
|-|-|  
|metadata|Information, such as location, time, message size, and/or exception information.|  
|[!INCLUDE[afproductnamelong](../../includes/afproductnamelong-md.md)]|The specifications for building BizTalk adapters using open standards based on Web services.|  
  
####  <a name="O"></a> O  
  
|||  
|-|-|  
|one-way|A message exchange pattern (MEP) in which the sender sends a message, but no response is returned by the receiver. In BizTalk Server, MEPs are referred to as communication patterns.|  
|outbound operation|An operation that is invoked by the adapter on the line-of-business system (LOB).|  
|output.cs|The default output file created by the ServiceModel Metadata Utility tool (svcutil.exe).|  
  
####  <a name="P"></a> P  
  
|||  
|-|-|  
|picklist|A field in a business component whose value is typically constrained to one of a set of values (akin to enumeration).|  
|proxy|In WCF, refers to a managed-code object that implements the service contract exposed by a service. The WCF service model is based on the use of such proxies. In the WCF service model, the service contract is expressed as a .NET interface.|  
  
####  <a name="R"></a> R  
  
|||  
|-|-|  
|request-response|A message exchange pattern (MEP) in which the sender sends a request message and expects a response message from the receiver. In BizTalk Server, MEPs are referred to as communication patterns. Depending on the messaging technology and the direction of the request message (inbound or outbound), this pattern is also called request-reply or solicit-response.|  
|run-time experience|Procedures and operations performed by a developer during run time or when deploying a solution; for example, creating a physical port binding from the BizTalk Server Administration console.|  
  
####  <a name="S"></a> S  
  
|||  
|-|-|  
|schema|The structure for a message. A schema can contain multiple subschema.|  
|ServiceModel Metadata Utility tool|A command-line utility that is included with WCF. It is used to create service model proxy code from the service description (metadata) that is exposed by a WCF service such as an adapter. For outbound operations, the tool creates a WCF client class and helper code; for inbound operations, the tool creates a WCF service contract and helper code.|  
|Siebel business component|Associates logically related columns from one or more tables into a single structure.|  
|Siebel business object|Represents a logical grouping of business components.|  
|Siebel business service|A collection of business service methods or functions that can be directly invoked in the Siebel system.|  
|Siebel COM Data Control library|Contains interfaces that enable an external client like the Siebel adapter to connect and communicate with a Siebel Application Object Manager on a Siebel server.|  
|Simple Object Access Protocol|See SOAP.|  
|SOAP|A simple, XML-based protocol for exchanging structured and type information in decentralized, distributed environments. WCF is based on the exchange of SOAP messages between clients and services to invoke operations and return results.|  
|SOAP message|A well-formed XML document. It should use the SOAP envelope and SOAP encoding namespaces and include an optional XML declaration, followed by a SOAP envelope (the root element), which is made up of an optional SOAP header and a SOAP message body.|  
|SQL Server Integration Services|A component that is used to import, export, and transform data from different data sources. Previously called data transformation service (DTS).|  
|SSIS|See SQL Server Integration Services.|  
|SSO|See Enterprise Single Sign-on system.|  
|strongly-typed data|A data set or result set that is bound to an underlying object type. Each row in a strongly-typed XML data set is composed of typed, named elements that correspond to fields of the underlying object type.|  
|svcutil|See ServiceModel Metadata Utility tool.|  
  
####  <a name="U"></a> U  
  
|||  
|-|-|  
|Uniform Resource Identifier (URI)|See connection URI.|  
  
####  <a name="W"></a> W  
  
|||  
|-|-|  
|WCF|See Windows Communication Foundation.|  
|WCF channel model|A programming model that relies on several interfaces and other types. Channels provide a low-level programming model for sending and receiving messages.|  
|WCF client|A client-application construct that exposes the service operations as methods. You can use the Add Adapter Service Reference Visual Studio Plug-in or the ServiceModel Metadata Utility Tool to generate a WCF client class from the metadata exposed by an adapter.|  
|[!INCLUDE[afproductnameshort](../../includes/afproductnameshort-md.md)]|See [!INCLUDE[afproductnamelong](../../includes/afproductnamelong-md.md)].|  
|WCF service contract|A managed-code representation of the service contract. It is expressed as an interface in which classes and methods are attributed to define the service, operation, message, and data contracts used to communicate with a service. You can use the ServiceModel Metadata Utility tool or the Add Adapter Service Reference Visual Studio Plug-in to generate a WCF service contract from the metadata exposed by an adapter. You implement the WCF service contract to receive operations from an LOB system.|  
|WCF service model|A WCF programming model in which a service is represented as a managed code object. The operations exposed by the service are represented as methods with strongly-typed data.|  
|weakly-typed data|A data set or result set that is not bound to an underlying object type. Each row in a weakly-typed XML data set is composed of a collection of generic columns in which attributes describe the name and type of each element.|  
|Web services|A unit of application logic providing data and services to other applications. Applications access XML Web services using standard Web protocols and data formats such as HTTP, XML, and SOAP, independent of how each XML Web service is implemented. XML Web services combine the best aspects of component-based development and the Web, and are a cornerstone of the Microsoft .NET programming model.|  
|Web Services Description Language|An XML-based language that describes a service as a set of endpoints that operate on messages. The WSDL document describes the service contract, operation contracts, message contracts, and data contracts that a client must use to interface with the service.|  
|Windows Communication Foundation (WCF)|A Microsoft service-oriented communication infrastructure. The framework inherently provides clients with a service programming model and a channel programming model for finer control of message exchanges.|  
|WSDL|See Web Services Description Language.|  
|WS-Metadata Exchange (MEX) endpoint|An endpoint exposed by a WCF service, such as an adapter, that implements the **IMetadataExchange** interface. A WS-Metadata Exchange endpoint can be used to retrieve a service description (WSDL) for operations exposed by an adapter on the target system.|  
  
####  <a name="X"></a> X  
  
|||  
|-|-|  
|XML|See Extensible Markup Language.|  
|XML Schema definition language (XSD)|A schema language. An XML Schema defines the elements, attributes, and data types that comply with the World Wide Web Consortium (W3C) XML Schema Part 1: Structures Recommendation for the XML Schema Definition Language. The W3C XML Schema Part 2: Datatypes Recommendation is the recommendation for defining data types that are used in XML schemas. The XML Schema definition language enables you to define the structure and data types for XML messages.|  
|XSD|See XML Schema definition language.|