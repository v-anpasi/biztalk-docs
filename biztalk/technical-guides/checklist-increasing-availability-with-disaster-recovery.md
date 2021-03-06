---
title: "Checklist: Increasing Availability with Disaster Recovery | Microsoft Docs"
ms.custom: ""
ms.date: "06/08/2017"
ms.prod: "biztalk-server-2013"
ms.reviewer: ""
ms.suite: ""
ms.tgt_pltfrm: ""
ms.topic: "article"
ms.assetid: 0b315110-206a-4fa7-9bde-abab1429c83b
caps.latest.revision: 3
author: "MandiOhlinger"
ms.author: "mandia"
manager: "anneta"
---
# Checklist: Increasing Availability with Disaster Recovery
This topic describes the steps that you should follow to increase availability of a production [!INCLUDE[btsBizTalkServerNoVersion](../includes/btsbiztalkservernoversion-md.md)] environment using disaster recovery. Disaster recovery is typically implemented after providing high availability with fault tolerance and/or load balancing.  
  
## Backing Up BizTalk Server  
  
|Step|Reference|  
|----------|---------------|  
|Keep a written record of all changes to your [!INCLUDE[btsBizTalkServerNoVersion](../includes/btsbiztalkservernoversion-md.md)] system.||  
|Ensure that you have appropriate permissions to back up and restore [!INCLUDE[btsBizTalkServerNoVersion](../includes/btsbiztalkservernoversion-md.md)].|See [Minimum Security User Rights](http://go.microsoft.com/fwlink/?LinkId=154374) (http://go.microsoft.com/fwlink/?LinkId=154374)|  
|Create a highly available file share for purposes of storing the [!INCLUDE[btsSQLServerNoVersion](../includes/btssqlservernoversion-md.md)] logs. Configure a highly available file share at the hardware level using a SAN and/or at the Windows Server level by using Windows Clustering.|See [How to create file shares on a cluster](http://support.microsoft.com/kb/224967) (http://support.microsoft.com/kb/224967)|  
|Install and make available one or more standby [!INCLUDE[btsSQLServerNoVersion](../includes/btssqlservernoversion-md.md)] instances as the destination for [!INCLUDE[btsBizTalkServerNoVersion](../includes/btsbiztalkservernoversion-md.md)] log shipping. The hardware for and the number of destination [!INCLUDE[btsSQLServerNoVersion](../includes/btssqlservernoversion-md.md)] instances should match the hardware for and number of [!INCLUDE[btsSQLServerNoVersion](../includes/btssqlservernoversion-md.md)] instances in the production environment. This will ensure that the destination [!INCLUDE[btsSQLServerNoVersion](../includes/btssqlservernoversion-md.md)] instance(s) can handle the same load as the production [!INCLUDE[btsSQLServerNoVersion](../includes/btssqlservernoversion-md.md)] instance(s).|See [Installing SQL Server 2008](http://go.microsoft.com/fwlink/?LinkId=154377) (http://go.microsoft.com/fwlink/?LinkId=154377)|  
|Prepare the disaster recovery site.|[Prepare the Disaster Recovery Site](../technical-guides/prepare-the-disaster-recovery-site.md)|  
|Back up and restore [!INCLUDE[btsBizTalkServerNoVersion](../includes/btsbiztalkservernoversion-md.md)] databases|-   [Best Practices for Backing Up and Restoring Databases](http://go.microsoft.com/fwlink/?LinkId=157758) (http://go.microsoft.com/fwlink/?LinkId=157758)<br />-   [Backing Up and Restoring BizTalk Server Databases](http://go.microsoft.com/fwlink/?LinkId=157757) (http://go.microsoft.com/fwlink/?LinkId=157757)|  
|Configure [!INCLUDE[btsBizTalkServerNoVersion](../includes/btsbiztalkservernoversion-md.md)] log shipping.|[Configuring BizTalk Server Log Shipping](../technical-guides/configuring-biztalk-server-log-shipping.md)|  
|Configure the Backup [!INCLUDE[btsBizTalkServerNoVersion](../includes/btsbiztalkservernoversion-md.md)] job.|[How to Configure the Backup BizTalk Server Job](http://go.microsoft.com/fwlink/?LinkID=154072) (http://go.microsoft.com/fwlink/?LinkID=154072)|  
|Configure the server where backups will be stored.|[How to Configure the Destination System for Log Shipping](http://go.microsoft.com/fwlink/?LinkID=151402) (http://go.microsoft.com/fwlink/?LinkID=151402)|  
|If you are using Business Activity Monitoring (BAM), back up the BAM databases.|[Backing Up the BAM Analysis and Tracking Analysis Server Databases](../technical-guides/backing-up-the-bam-analysis-and-tracking-analysis-server-databases.md)|  
|If you are using BAM, back up the BAM portal application pools and virtual directories configuration information. If you are not using BAM, you do not need to perform this step.|[How to Back Up the BAM Portal](http://go.microsoft.com/fwlink/?LinkId=154378) (http://go.microsoft.com/fwlink/?LinkId=154378)|  
|Back up the [!INCLUDE[btsBizTalkServerNoVersion](../includes/btsbiztalkservernoversion-md.md)] configuration file.|[How to Back Up The BizTalk Server Configuration](http://go.microsoft.com/fwlink/?LinkId=154379) (http://go.microsoft.com/fwlink/?LinkId=154379)|  
|If you are using Enterprise Single Sign-on, back up the master secret server.|[How to Back Up the Master Secret](http://go.microsoft.com/fwlink/?LinkID=151395) (http://go.microsoft.com/fwlink/?LinkID=151395)|  
  
## Restoring BizTalk Server  
  
|Steps|Reference|  
|-----------|---------------|  
|Restore the BizTalk group.|[Restoring the BizTalk Group](../technical-guides/restoring-the-biztalk-group.md)|  
|Recover the run-time computers running [!INCLUDE[btsBizTalkServerNoVersion](../includes/btsbiztalkservernoversion-md.md)].|[Recovering the Runtime Computers](../technical-guides/recovering-the-runtime-computers.md)|  
|Recover BAM alerts.|[How to Recover BAM Alerts](http://go.microsoft.com/fwlink/?LinkId=154380) (http://go.microsoft.com/fwlink/?LinkId=154380)|  
|Recover the BAM portal.|[How to Recover the BAM Portal](http://go.microsoft.com/fwlink/?LinkId=154381) (http://go.microsoft.com/fwlink/?LinkId=154381)|  
|Restore the master secret server.|[How to Restore the Master Secret](http://go.microsoft.com/fwlink/?LinkId=151394) (http://go.microsoft.com/fwlink/?LinkId=151394)|  
|Restore the [!INCLUDE[btsBizTalkServerNoVersion](../includes/btsbiztalkservernoversion-md.md)] databases.|[How to Restore Your Databases](http://go.microsoft.com/fwlink/?LinkId=151406) (http://go.microsoft.com/fwlink/?LinkId=151406)|  
|Update references to the BAM database names.|-   [Updating References to the New BAM Primary Import Database](../technical-guides/how-to-move-the-bam-primary-import-database2.md#BKMK_BAMPIRef)<br />-   [Updating References to the New BAM Archive Database](../technical-guides/how-to-move-the-bam-archive-database1.md#BKMK_UpdateArch)<br />-   [Updating References to the New BAM Star Schema Database](../technical-guides/how-to-move-the-bam-star-schema-database2.md#BKMK_StarUpdate)<br />-   [Updating References to the New BAM Analysis Database](../technical-guides/how-to-move-the-bam-analysis-database1.md#BKMK_AnalyUpdate)<br />-   [Updating References to the New BAM Notification Services Databases](../technical-guides/how-to-move-the-bam-notification-services-databases1.md#BKMK_NotiUpdate)<br />-   [How to Resolve Incomplete Activity Instances](http://go.microsoft.com/fwlink/?LinkId=151475) (http://go.microsoft.com/fwlink/?LinkId=151475)|  
  
## See Also  
 [Disaster Recovery](../technical-guides/disaster-recovery.md)