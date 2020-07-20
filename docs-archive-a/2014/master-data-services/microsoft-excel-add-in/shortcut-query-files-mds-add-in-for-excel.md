---
title: "Shortcut Query Files (MDS Add-in for Excel) | Microsoft Docs"
ms.custom: ""
ms.date: "03/06/2017"
ms.prod: "sql-server-2014"
ms.reviewer: ""
ms.technology: master-data-services
ms.topic: conceptual
ms.assetid: 1ba0219a-6c40-41fa-aff9-8c8f41ef3220
author: lrtoyou1223
ms.author: lle
---
# Shortcut Query Files (MDS Add-in for Excel)
  In the [!INCLUDE[ssMDSshort](../../includes/ssmdsshort-md.md)][!INCLUDE[ssMDSXLS](../../includes/ssmdsxls-md.md)], use shortcut query files to quickly connect and load frequently-used data. You can also use them when you want to share MDS data with others. Instead of saving the worksheet and emailing it, you should save a shortcut query file and email that instead. This ensures that you are both connecting to the MDS repository to get the latest data.  
  
 Shortcut query files are XML files that contain information about:  
  
-   The MDS repository connection.  
  
-   The model, version, and entity.  
  
-   Any filters that were applied when the shortcut was created.  
  
-   The left-to-right order of the columns when the shortcut was created.  
  
 You can save these files in a list and choose from them when you open the Add-in. You can export them to your computer or to a shared location, or you can send them to others.  
  
## QueryOpener Application  
 All users who install the [!INCLUDE[ssMDSXLS](../../includes/ssmdsxls-md.md)] have an application called QueryOpener installed. This application is used to open shortcut query files in the [!INCLUDE[ssMDSXLS](../../includes/ssmdsxls-md.md)]. If you double-click a shortcut query file, this application is automatically used to open the file in the Add-in.  
  
 When you open a shortcut query file with this application, you are prompted to make the connection a "safe" connection, which means you trust content from this location. Each time you mark a connection as safe, it is added to a list. If you want to clear this list, open the **Settings** dialog box and in the **Servers Added to Safe List** section, click **Clear All**.  
  
 The default location for the application is *drive*:\Program Files\Microsoft SQL Server\120\Master Data Services\Excel Add-In\Microsoft.MasterDataServices.QueryOpener.exe.  
  
 There are two ways to open shortcut query files: you can import them or you can double-click them and they are opened automatically.  
  
## Related Tasks  
  
|Task Description|Topic|  
|----------------------|-----------|  
|Save the contents of the active worksheet as a shortcut query file.|[Save a Shortcut Query File &#40;MDS Add-in for Excel&#41;](save-a-shortcut-query-file-mds-add-in-for-excel.md)|  
|Email a shortcut query file that represents the contents of the active worksheet.|[Email a Shortcut Query File &#40;MDS Add-in for Excel&#41;](email-a-shortcut-query-file-mds-add-in-for-excel.md)|  
  
## Related Content  
  
-   [Connections &#40;MDS Add-in for Excel&#41;](connections-mds-add-in-for-excel.md)  
  
-   [Master Data Services Add-in for Microsoft Excel](master-data-services-add-in-for-microsoft-excel.md)  
  
-   [Security &#40;Master Data Services&#41;](../security-master-data-services.md)  
  
  