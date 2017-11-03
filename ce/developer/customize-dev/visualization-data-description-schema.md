---
title: "Visualization data description schema (Developer Guide for Dynamics 365 Customer Engagement) | MicrosoftDocs"
description: "The following is the schema for the data description XML string for charts in visualization. This can be used to validate the contents of the data description XML string while creating a chart. "
ms.custom: ""
ms.date: 10/31/2017
ms.reviewer: ""
ms.service: "crm-online"
ms.suite: ""
ms.tgt_pltfrm: ""
ms.topic: "article"
applies_to: 
    - "Dynamics 365 (online)"
ms.assetid: c923e9fd-c687-4671-9ffd-1306da9f80d8
caps.latest.revision: 14
author: "KumarVivek"
ms.author: "kvivek"
manager: "amyla"
---
# Visualization data description schema

[!INCLUDE[](../../includes/cc_applies_to_update_9_0_0.md)]

The following is the schema for the data description XML string for charts in visualization. This can be used to validate the contents of the data description XML string while creating a chart. For more information, see [Understanding Charts: Underlying Data and Chart Representation](understand-charts-underlying-data-chart-representation.md). You can find this schema in the `SDK\Schemas\VisualizationDataDescription.xsd` file in the SDK [!INCLUDE[sdk_download](../../includes/sdk-download.md)] package.  
  
## Schema  
  
```xml  
<?xml version='1.0' encoding='utf-8'?>  
<xs:schema attributeFormDefault='unqualified'  
           elementFormDefault='qualified'  
           xmlns:xs='http://www.w3.org/2001/XMLSchema'>  
 <xs:element name='datadefinition'>  
  <xs:complexType>  
   <xs:sequence>  
    <xs:element name='fetchcollection'>  
     <xs:complexType>  
      <xs:sequence>  
       <xs:element maxOccurs='unbounded'  
                   name='fetch'>  
        <xs:annotation>  
         <!--FetchXML goes here-->  
        </xs:annotation>  
       </xs:element>  
      </xs:sequence>  
     </xs:complexType>  
    </xs:element>  
    <xs:element name='categorycollection'>  
     <xs:complexType>  
      <xs:sequence>  
       <xs:element name='category'  
                   type='CategoryType'  
                   minOccurs='1'  
                   maxOccurs='unbounded' />  
      </xs:sequence>  
     </xs:complexType>  
    </xs:element>  
   </xs:sequence>  
  </xs:complexType>  
 </xs:element>  
 <xs:complexType name ='CategoryType'>  
  <xs:sequence>  
   <xs:element minOccurs='1'  
               maxOccurs='unbounded'  
               name='measurecollection'>  
    <xs:complexType>  
     <xs:sequence>  
      <xs:element minOccurs='1'  
                  maxOccurs='unbounded'  
                  name='measure'>  
       <xs:complexType>  
        <xs:attribute name='alias'  
                      type='xs:string'  
                      use='required' />  
       </xs:complexType>  
      </xs:element>  
     </xs:sequence>  
    </xs:complexType>  
   </xs:element>  
  </xs:sequence>  
  <xs:attribute name='alias'  
                type='xs:string'  
                use='optional' />  
 </xs:complexType>  
</xs:schema>  
```  
  
### See also  
 [Customize Visualizations and Dashboards](customize-visualizations-dashboards.md)   
 [Schemas Used in Microsoft Dynamics 365](../schemas-used-dynamics-365.md)   
 [Understanding Charts: Underlying Data and Chart Representation](understand-charts-underlying-data-chart-representation.md)   
 [Sample Charts](sample-charts.md)   
 [Use FetchXML to Construct a Query](../org-service/use-fetchxml-construct-query.md)