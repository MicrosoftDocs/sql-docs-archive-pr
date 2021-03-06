---
description: "Some availability replicas do not have a healthy role"
title: "Some availability replicas do not have a healthy role | Microsoft Docs"
ms.custom: ""
ms.date: "06/13/2017"
ms.prod: "sql-server-2014"
ms.reviewer: ""
ms.technology: high-availability
ms.topic: conceptual
f1_keywords: 
  - "sql12.swb.agdashboard.agp6allroleshealthy.issues.f1"
helpviewer_keywords: 
  - "Availability Groups [SQL Server], policies"
ms.assetid: 7ec5b337-7201-4a66-a541-7560f8b18784
author: MashaMSFT
ms.author: mathoma
---
# Some availability replicas do not have a healthy role
    
## Introduction  
  
|||  
|-|-|  
|**Policy Name**|Availability Replicas Role State|  
|**Issue**|Some availability replicas do not have a healthy role.|  
|**Category**|**Warning**|  
|**Facet**|Availability group|  
  
## Description  
 This policy rolls up the connection state of all availability replicas and checks if there are any availability replicas that are not in a healthy role. The policy is in an unhealthy state when any availability replica is neither primary nor secondary. The policy is otherwise in a healthy state.  
  
> [!NOTE]  
>  For this release of [!INCLUDE[ssCurrent](../../../includes/sscurrent-md.md)], information about possible causes and solutions is located at [Some availability replicas do not have a healthy role](https://go.microsoft.com/fwlink/p/?LinkId=220854) on the TechNet Wiki.  
  
## Possible Causes  
 In this availability group, at least one availability replica does not currently have the primary or secondary role.  
  
## Possible Solution  
 Use the availability replica policy state to find the availability replica whose role is not primary or secondary, and then resolve the issue at the availability replica.  
  
## See Also  
 [Overview of AlwaysOn Availability Groups &#40;SQL Server&#41;](overview-of-always-on-availability-groups-sql-server.md)   
 [Use the AlwaysOn Dashboard &#40;SQL Server Management Studio&#41;](use-the-always-on-dashboard-sql-server-management-studio.md)  
  
  
