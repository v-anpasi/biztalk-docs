---
title: "Performance Tools | Microsoft Docs"
ms.custom: ""
ms.date: "06/08/2017"
ms.prod: "biztalk-server-2013"
ms.reviewer: ""
ms.suite: ""
ms.tgt_pltfrm: ""
ms.topic: "article"
ms.assetid: 6d26c17a-3eb9-41a5-b0dc-31b974bf3d9b
caps.latest.revision: 11
author: "MandiOhlinger"
ms.author: "mandia"
manager: "anneta"
---
# Performance Tools
This topic provides information on tools you can use to evaluate the performance of a BizTalk Server solution. The tools described in this topic have different purposes; some are designed to evaluate end-to-end performance while others focus on evaluating performance of a particular aspect of a BizTalk Server solution.  
  
## BizTalk Server Orchestration Profiler  
 The BizTalk Server Orchestration Profiler is used to view orchestration tracking data for a specified period of time and is useful for determining where performance bottlenecks exist in orchestrations.  
  
 For more information about the BizTalk Server Orchestration Profiler, see [BizTalk Server 2006 Orchestration Profiler](http://go.microsoft.com/fwlink/?LinkId=102209) (http://go.microsoft.com/fwlink/?LinkId=102209).  
  
> [!NOTE]  
>  Use of this tool is not supported by Microsoft, and Microsoft makes no guarantees about the suitability of this programs. Use of this program is entirely at your own risk. Also note that this utility was designed to work with BizTalk Server 2006 and therefore may not work as expected on BizTalk Server 2010.  
  
## BizUnit 3.0 and BizUnit Designer  
 BizUnit is a framework designed for automated testing of BizTalk solutions. BizUnit is an excellent tool for testing end-to-end BizTalk Server scenarios. Performing automated testing of BizTalk solutions with BizUnit is the primary focus of the [Implementing Automated Testing](../technical-guides/implementing-automated-testing.md) section of this guide. For more information about BizUnit 3.0, see [BizUnit - Framework for Automated Testing of Distributed Systems](http://go.microsoft.com/fwlink/?LinkID=85168) (http://go.microsoft.com/fwlink/?LinkID=85168).  
  
 BizUnit Designer is a GUI that allows for rapid creation of BizUnit test cases that can be used for unit testing or system testing distributed applications. The tool is available at [BizUnit Designer](http://go.microsoft.com/fwlink/?LinkID=117917) (http://go.microsoft.com/fwlink/?LinkID=117917).  
  
> [!IMPORTANT]  
>  As of the writing of this guide, the test cases generated by BizUnit Designer 1.x are only compatible with BizUnit 2.x.  
  
> [!NOTE]  
>  Use of this tool is not supported by Microsoft, and Microsoft makes no guarantees about the suitability of this programs. Use of this program is entirely at your own risk.  
  
## IOMeter  
 IOMeter is an open source tool used for measuring disk I/O performance. For more information about IOMeter, see [http://www.iometer.org](http://go.microsoft.com/fwlink/?LinkId=122412) (http://go.microsoft.com/fwlink/?LinkId=122412).  
  
> [!NOTE]  
>  Use of this tool is not supported by Microsoft, and Microsoft makes no guarantees about the suitability of this programs. Use of this program is entirely at your own risk.  
  
## Log Parser  
 Log parser is a powerful, versatile tool that provides universal query access to text-based data such as log files, XML files and CSV files, as well as key data sources on the Windows® operating system such as the Event Log, the Registry, the file system, and Active Directory®. Log Parser is available for download at [Log Parser 2.2](http://go.microsoft.com/fwlink/?LinkID=100882) (http://go.microsoft.com/fwlink/?LinkID=100882).  
  
## Microsoft BizTalk LoadGen 2007  
 BizTalk LoadGen 2007 is a load generation tool used to run performance and stress tests against [!INCLUDE[btsBizTalkServer2006r3](../includes/btsbiztalkserver2006r3-md.md)].  
  
 For more information about the Microsoft BizTalk LoadGen 2007 tool, see [Microsoft BizTalk LoadGen 2007 Tools](http://go.microsoft.com/fwlink/?LinkId=59841) (http://go.microsoft.com/fwlink/?LinkId=59841).  
  
## Pathping  
 Pathping provides information about possible data loss at one or more router hops on the way to a target host. To do so, pathping sends Internet Control Message Protocol (ICMP) packets to each router in the path. Pathping.exe is available with all versions of Windows since Windows 2000 Server.  
  
## Performance Analysis of Logs (PAL)  
 The PAL tool is used to generate an HTML-based report that graphically charts important performance counters and generates alerts when thresholds for these counters are exceeded. PAL is an excellent tool for identifying bottlenecks in a BizTalk Server solution to facilitate the appropriate allocation of resources when optimizing the performance of the solution.  
  
 For more information about the Performance Analysis of Logs (PAL) tool, see [Performance Analysis of Logs (PAL) Tool](http://go.microsoft.com/fwlink/?LinkID=98098) (http://go.microsoft.com/fwlink/?LinkID=98098).  
  
> [!NOTE]  
>  Use of this tool is not supported by Microsoft, and Microsoft makes no guarantees about the suitability of this programs. Use of this program is entirely at your own risk.  
  
## Performance Monitor  
 Performance Monitor provides a visual display of built-in Windows performance counters, either in real time or as a way to review historical data.  
  
## Relog  
 The Relog utility is used to extract performance counters from logs created by Performance Monitor and convert the data into other formats, such as tab-delimited text files (text-TSV), comma-delimited text files (text-CSV), binary files, and SQL databases. This data can then be analyzed and queried using other tools, such as Log Parser, to generate statistics for key performance indicators (KPIs). The Relog utility is provided with [!INCLUDE[btsWinSvr2k3](../includes/btswinsvr2k3-md.md)] and subsequent versions.  
  
## Visual Studio 2010 - Testing the Application  
 Both Microsoft Visual Studio 2010 Ultimate and Visual Studio Test Professional 2010 now include a new application called Microsoft Test Manager to help you define and manage your testing effort by using test plans. For more information about working with load tests, see [Testing the Application](http://go.microsoft.com/fwlink/?LinkID=205342) (http://go.microsoft.com/fwlink/?LinkID=205342).  
  
## Visual Studio 2010 Profiling Tools  
 The Visual Studio Profiling Tools allows you to profile custom .NET components (custom pipeline components, helper components invoked by pipelines and\or orchestrations, custom functoids). For more information about Visual Studio Profiling Tools see, [Analyzing Application Performance by Using Profiling Tools](http://go.microsoft.com/fwlink/?LinkID=210555) (http://go.microsoft.com/fwlink/?LinkID=210555).  
  
## Windows Performance Analysis Tools  
 Windows Performance Tools are designed for analysis of a wide range of performance problems including application start times, boot issues, deferred procedure calls and interrupt activity (DPCs and ISRs), system responsiveness issues, application resource usage, and interrupt storms.  
  
 For more information about the Windows Performance Analysis Tools, see [Windows Performance Analysis](http://go.microsoft.com/fwlink/?LinkId=139763) (http://go.microsoft.com/fwlink/?LinkId=139763).  
  
## SQL Server Tools for Performance Monitoring and Tuning  
 [!INCLUDE[btsSQLServerNoVersion](../includes/btssqlservernoversion-md.md)] provides several tools for monitoring events in [!INCLUDE[btsSQLServerNoVersion](../includes/btssqlservernoversion-md.md)] and for tuning the physical database design. These tools are described in the [!INCLUDE[btsSQLServerNoVersion](../includes/btssqlservernoversion-md.md)] Books Online topic [Tools for Performance Monitoring and Tuning](http://go.microsoft.com/fwlink/?LinkId=146357) (http://go.microsoft.com/fwlink/?LinkId=146357). Information about specific tools used for [!INCLUDE[btsSQLServerNoVersion](../includes/btssqlservernoversion-md.md)] performance monitoring and tuning is provided below:  
  
### SQL Profiler  
 Microsoft [!INCLUDE[btsSQLServerNoVersion](../includes/btssqlservernoversion-md.md)] Profiler can be used to capture Transact-SQL statements that are sent to [!INCLUDE[btsSQLServerNoVersion](../includes/btssqlservernoversion-md.md)] and the [!INCLUDE[btsSQLServerNoVersion](../includes/btssqlservernoversion-md.md)] result sets from these statements. Because [!INCLUDE[btsSQLServerNoVersion](../includes/btssqlservernoversion-md.md)] is tightly integrated with [!INCLUDE[btsSQLServerNoVersion](../includes/btssqlservernoversion-md.md)], the analysis of a [!INCLUDE[btsSQLServerNoVersion](../includes/btssqlservernoversion-md.md)] Profile trace can be a useful tool for analyzing problems that may occur in [!INCLUDE[btsBizTalkServerNoVersion](../includes/btsbiztalkservernoversion-md.md)] when reading from and writing to [!INCLUDE[btsSQLServerNoVersion](../includes/btssqlservernoversion-md.md)] databases. For information about how to use [!INCLUDE[btsSQLServerNoVersion](../includes/btssqlservernoversion-md.md)] Profiler, see the [!INCLUDE[btsSQLServer2008R2](../includes/btssqlserver2008r2-md.md)] Books Online topic [Using SQL Server Profiler](http://go.microsoft.com/fwlink/?linkid=104423) (http://go.microsoft.com/fwlink/?linkid=104423).  
  
> [!IMPORTANT]  
>  There is considerable overhead associated with running SQL Profiler. Therefore SQL Profiler is best suited for use in test or development environments. If using SQL Profiler to troubleshoot a production environment, be aware of the associated overhead costs and limit the use of SQL Profiler accordingly.  
  
> [!NOTE]  
>  When using SQL Profiler to capture Transact-SQL statements, configure SQL Profiler to generate output to a local drive rather than a drive located on a remote network share or other slow device, for example, a local USB memory stick.  
  
### SQL Trace  
 [!INCLUDE[btsSQLServerNoVersion](../includes/btssqlservernoversion-md.md)] provides Transact-SQL system stored procedures to create traces on an instance of the SQL Server Database Engine. These system stored procedures can be used from within your own applications to create traces manually, instead of using SQL Server Profiler. This allows you to write custom applications specific to the needs of your enterprise. For more information about using SQL Trace, see the [!INCLUDE[btsSQLServer2008R2](../includes/btssqlserver2008r2-md.md)] Books Online topic [Introducing SQL Trace](http://go.microsoft.com/fwlink/?LinkId=146354) (http://go.microsoft.com/fwlink/?LinkId=146354).  
  
> [!NOTE]  
>  When using SQL Trace to capture Transact-SQL statements, configure SQL Trace to generate output to a local drive rather than a drive located on a remote network share or other slow device, such as a USB flash drive.  
  
### SQL Activity Monitor  
 [!INCLUDE[btsSQLServer2008R2](../includes/btssqlserver2008r2-md.md)] Activity Monitor provides information about [!INCLUDE[btsSQLServerNoVersion](../includes/btssqlservernoversion-md.md)] processes and how these processes affect the current instance of [!INCLUDE[btsSQLServerNoVersion](../includes/btssqlservernoversion-md.md)]. For more information about [!INCLUDE[btsSQLServer2008R2](../includes/btssqlserver2008r2-md.md)] Activity Monitor, see the [!INCLUDE[btsSQLServer2008R2](../includes/btssqlserver2008r2-md.md)] Books Online topic [Activity Monitor](http://go.microsoft.com/fwlink/?LinkId=146355) (http://go.microsoft.com/fwlink/?LinkId=146355). For information about how to open Activity Monitor from [!INCLUDE[btsSQLServerNoVersion](../includes/btssqlservernoversion-md.md)] Management Studio, see the [!INCLUDE[btsSQLServer2008R2](../includes/btssqlserver2008r2-md.md)] Books Online topic [How to: Open Activity Monitor (SQL Server Management Studio)](http://go.microsoft.com/fwlink/?LinkId=135094) (http://go.microsoft.com/fwlink/?LinkId=135094).  
  
### SQL Server 2008 R2 Data Collection  
 [!INCLUDE[btsSQLServer2008R2](../includes/btssqlserver2008r2-md.md)] provides a data collector that you can use to obtain and save data that is gathered from several sources. The data collector enables you to use data collection containers, which enable you to determine the scope and frequency of data collection on a computer that is running [!INCLUDE[btsSQLServer2008R2](../includes/btssqlserver2008r2-md.md)]. For more information about implementing [!INCLUDE[btsSQLServer2008R2](../includes/btssqlserver2008r2-md.md)] data collection, see the [!INCLUDE[btsSQLServer2008R2](../includes/btssqlserver2008r2-md.md)] Books Online topic [Data Collection](http://go.microsoft.com/fwlink/?LinkId=146356) (http://go.microsoft.com/fwlink/?LinkId=146356).  
  
### SQLIO  
 The SQLIO tool was developed by Microsoft to evaluate the I/O capacity of a given configuration. As the name of the tool implies, SQLIO is a valuable tool for measuring the impact of file system I/O on [!INCLUDE[btsSQLServerNoVersion](../includes/btssqlservernoversion-md.md)] performance. SQLIO can be downloaded from [SQLIO Disk Subsystem Benchmark Tool](http://go.microsoft.com/fwlink/?LinkId=115176) (http://go.microsoft.com/fwlink/?LinkId=115176).  
  
## See Also  
 [Finding and Eliminating Bottlenecks](../technical-guides/finding-and-eliminating-bottlenecks.md)