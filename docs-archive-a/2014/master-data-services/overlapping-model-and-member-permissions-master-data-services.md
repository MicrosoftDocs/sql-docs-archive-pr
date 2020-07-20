---
title: "Overlapping Model and Member Permissions (Master Data Services) | Microsoft Docs"
ms.custom: ""
ms.date: "03/06/2017"
ms.prod: "sql-server-2014"
ms.reviewer: ""
ms.technology: master-data-services
ms.topic: conceptual
helpviewer_keywords: 
  - "models [Master Data Services], effective permissions"
  - "permissions [Master Data Services], model and member overlaps"
  - "members [Master Data Services], effective permissions"
ms.assetid: 9fd7a555-43bf-4796-a8b6-1ca63a291216
author: lrtoyou1223
ms.author: lle
---
# Overlapping Model and Member Permissions (Master Data Services)
  Permission assigned to a member can overlap with permission assigned to a model object. When overlaps occur, the more restrictive permission takes effect.  
  
 If a member has permission that is different than its corresponding model object, the following rules apply:  
  
-   **Deny** overrides all other permissions.  
  
-   **Read-only** overrides **Update**.  
  
 The following image shows which permissions take effect on an individual attribute value when attribute permissions are different than member permissions.  
  
 ![mds_conc_security_member_overlap_table](../../2014/master-data-services/media/mds-conc-security-member-overlap-table.gif "mds_conc_security_member_overlap_table")  
  
## Example 1  
 ![mds_conc_overlap_model_1](../../2014/master-data-services/media/mds-conc-overlap-model-1.gif "mds_conc_overlap_model_1")  
  
 On the **Models** tab, the Product entity has **Update** permission assigned. All attributes in the entity inherit that permission.  
  
 On the **Hierarchy Members** tab, the Mountain Bikes subcategory node in a derived hierarchy has **Update** permission assigned.  
  
 Result: In **Explorer**, the user has **Update** permission to all attribute values for all members in the Mountain Bikes node. All other members and attributes are hidden.  
  
 ![mds_conc_overlap_model_example_1](../../2014/master-data-services/media/mds-conc-overlap-model-example-1.gif "mds_conc_overlap_model_example_1")  
  
## Example 2  
 ![mds_conc_overlap_model_2](../../2014/master-data-services/media/mds-conc-overlap-model-2.gif "mds_conc_overlap_model_2")  
  
 On the **Models** tab, the Subcategory attribute has **Update** permission assigned.  
  
 On the **Hierarchy Members** tab, the Mountain Bikes subcategory node in a derived hierarchy is explicitly assigned **Read-only** permission.  
  
 Result: In **Explorer**, the user has **Read-only** permission to the Subcategory attribute values for the members in the Mountain Bikes node. All other members and attributes are hidden.  
  
 ![mds_conc_overlap_model_example_2](../../2014/master-data-services/media/mds-conc-overlap-model-example-2.gif "mds_conc_overlap_model_example_2")  
  
## Example 3  
 ![mds_conc_overlap_model_3](../../2014/master-data-services/media/mds-conc-overlap-model-3.gif "mds_conc_overlap_model_3")  
  
 On the **Models** tab, the Subcategory attribute has **Read-only** permission assigned.  
  
 On the **Hierarchy Members** tab, the Mountain Bikes subcategory in a derived hierarchy is explicitly assigned **Update** permission.  
  
 Result: In **Explorer**, the user has **Read-only** permission to the attribute values. All other members and attributes are hidden.  
  
 ![mds_conc_overlap_model_example_2](../../2014/master-data-services/media/mds-conc-overlap-model-example-2.gif "mds_conc_overlap_model_example_2")  
  
## See Also  
 [How Permissions Are Determined &#40;Master Data Services&#41;](how-permissions-are-determined-master-data-services.md)   
 [Overlapping User and Group Permissions &#40;Master Data Services&#41;](../../2014/master-data-services/overlapping-user-and-group-permissions-master-data-services.md)  
  
  