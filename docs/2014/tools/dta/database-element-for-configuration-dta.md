---
title: "Database Element for Configuration (DTA) | Microsoft Docs"
ms.custom: ""
ms.date: "06/13/2017"
ms.prod: "sql-server-2014"
ms.reviewer: ""
ms.suite: ""
ms.technology: 
  - "database-engine"
ms.tgt_pltfrm: ""
ms.topic: "article"
dev_langs: 
  - "XML"
helpviewer_keywords: 
  - "Database element"
ms.assetid: e91ba243-6cc9-457a-8f5a-134f3c71ae69
caps.latest.revision: 12
author: "craigg-msft"
ms.author: "craigg"
manager: "jhubbard"
---
# Database Element for Configuration (DTA)
  Specifies the database against which you want the Database Engine Tuning Advisor to evaluate the hypothetical configuration (specified by the `Configuration` element).  
  
## Syntax  
  
```  
  
<Server>  
...code removed here...  
    <Database>...</Database>  
```  
  
## Element Characteristics  
  
|Characteristic|Description|  
|--------------------|-----------------|  
|**Data type and length**|None.|  
|**Default value**|None.|  
|**Occurrence**|Required one or more times per `Server` element.|  
  
## Element Relationships  
  
|Relationship|Elements|  
|------------------|--------------|  
|**Parent element**|[Server Element for Configuration &#40;DTA&#41;](server-element-for-configuration-dta.md)|  
|**Child elements**|[Name Element for Database &#40;DTA&#41;](name-element-for-database-dta.md)<br /><br /> [Schema Element for Database &#40;DTA&#41;](schema-element-for-database-dta.md)<br /><br /> [Recommendation Element &#40;DTA&#41;](recommendation-element-dta.md)|  
  
## Remarks  
 This element is of the **DatabaseTypecomplexType** name in the Database Engine Tuning Advisor XML schema. Do not confuse this `Database` element with the one whose root parent is the `Server` element, which occurs at the top of the XML input file. For more information, see [Database Element for Server &#40;DTA&#41;](database-element-for-server-dta.md).  
  
## Example  
 For a usage example of this `Database` element, see the [XML Input File Sample with User-specified Configuration &#40;DTA&#41;](xml-input-file-sample-with-user-specified-configuration-dta.md).  
  
## See Also  
 [XML Input File Reference &#40;Database Engine Tuning Advisor&#41;](xml-input-file-reference-database-engine-tuning-advisor.md)  
  
  