---
title: "DISCOVER_PARTITION_DIMENSION_STAT Rowset | Microsoft Docs"
ms.date: 05/03/2018
ms.prod: sql
ms.technology: analysis-services
ms.component: schema-rowsets
ms.topic: reference
ms.author: owend
ms.reviewer: owend
author: minewiskan
manager: kfile
---
# DISCOVER_PARTITION_DIMENSION_STAT Rowset
[!INCLUDE[ssas-appliesto-sqlas](../../../includes/ssas-appliesto-sqlas.md)]
  Returns statistics on the dimension that is associated with a partition  
  
 **Applies to:** tabular models, multidimensional models  
  
## Rowset Columns  
 The **DISCOVER_PARTITION_DIMENSION_STAT** rowset contains the following columns.  
  
|Column name|Type indicator|Restriction|Description|  
|-----------------|--------------------|-----------------|-----------------|  
|**DATABASE_NAME**|**DBTYPE_WSTR**|Required|The name of the database.<br /><br /> This column is required in the restriction list.|  
|**CUBE_NAME**|**DBTYPE_WSTR**|Required|The name of the cube or tabular model.<br /><br /> This column is required in the restriction list.|  
|**MEASURE_GROUP_NAME**|**DBTYPE_WSTR**|Required|The name of the measure group.<br /><br /> This column is required in the restriction list.|  
|**PARTITION_NAME**|**DBTYPE_WSTR**|Required|The name of the partition.<br /><br /> This column is required in the restriction list.|  
|**DIMENSION_NAME**|**DBTYPE_WSTR**||The name of the dimension.<br /><br /> This column is required in the restriction list.|  
|**ATTRIBUTE_NAME**|**DBTYPE_WSTR**||The name of an attribute in the dimension.|  
|**ATTRIBUTE_INDEXED**|**DBTYPE_BOOL**||When true, indicates that the attribute is indexed; otherwise false.|  
|**ATTRIBUTE_COUNT_MIN**|**DBTYPE_I8**||The minimum attribute count.|  
|**ATTRIBUTE_COUNT_MAX**|**DBTYPE_I8**||The maximum attribute count.|  
  
 This schema rowset is not sorted.  
  
## Using ADOMD.NET to return the rowset  
 When using ADOMD.NET and the schema rowset to retrieve metadata, you can use either the GUID or string to reference a schema rowset object in the GetSchemaDataSet method. For more information, see [Working with Schema Rowsets in ADOMD.NET](../../../analysis-services/multidimensional-models-adomd-net-client/retrieving-metadata-working-with-schema-rowsets.md).  
  
 The following table provides the GUID and string values that identify this rowset.  
  
|Argument|Value|  
|--------------|-----------|  
|GUID|a07ccd8e-8148-11d0-87bb-00c04fc33942|  
|ADOMDNAME|PartitionDimensionStat|  
  
## See Also  
 [XML for Analysis Schema Rowsets](../../../analysis-services/schema-rowsets/xml/xml-for-analysis-schema-rowsets.md)  
  
  
