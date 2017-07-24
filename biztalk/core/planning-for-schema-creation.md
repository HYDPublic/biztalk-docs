---
title: "Planning for Schema Creation | Microsoft Docs"
ms.custom: ""
ms.date: "06/08/2017"
ms.prod: "biztalk-server"
ms.reviewer: ""
ms.service: "biztalk-server"
ms.suite: ""
ms.tgt_pltfrm: ""
ms.topic: "article"
ms.assetid: 4ecb9154-b457-4209-b9b9-572c186bf5e7
caps.latest.revision: 7
author: "MandiOhlinger"
ms.author: "mandia"
manager: "anneta"
---
# Planning for Schema Creation
You use schemas to validate instances of messages that are meant to conform to the schema, to define how instance messages in different formats (XML and non-XML) can be translated back and forth, and to define how XML instance messages with one structure can be transformed into XML instance messages with a different structure. For more information about the distinction between instance message translation and instance message transformation, see [Transformation vs. Translation](../core/data-transformation.md).  
  
 The following table lists some of the questions that you need to answer in planning for schema creation in BizTalk Editor.  
  
|Planning question|Recommendation|  
|-----------------------|--------------------|  
|What schemas do I need to create?|Make a list of the business documents that you will be processing using Microsoft [!INCLUDE[btsBizTalkServerNoVersion](../includes/btsbiztalkservernoversion-md.md)]. Such a list might include, for example, a purchase order, an invoice, a shipping confirmation, and so on. The list might also include more than one of each business document, such as when the structure of a purchase order you receive from one trading partner is different than the structure of a purchase order you receive from another trading partner.|  
|Are the documents I send and receive already represented as XML?|Add information to your list of documents regarding the format of each business document you send and receive, be it XML or some other format such as a delimited or positional flat file format.|  
|What starting points are available for the creation of the schemas on my list?|Although sometimes necessary, creating schemas is more difficult than generating them from one of the supported sources. If your schema is already represented in XML Schema definition (XSD) language, no generation is necessary and you can simply open it in BizTalk Editor.<br /><br /> If you have a well-formed XML instance message, a Document Type Definition (DTD) representation of your schema, or an XML-Data reduced (XDR) representation of your schema, you can automatically generate your schema. You may need to refine the generated schema using BizTalk Editor, but you will have saved yourself some work. For step-by-step instructions, see the procedure "To generate a schema from a non-XSD source" in [Creating Schemas for XML Messages](../core/how-to-create-schemas-for-xml-messages.md).<br /><br /> If none of these starting points are available to you for one or more of the business documents on your list, you will need to create a new schema using BizTalk Editor and define its structure.|  
  
## See Also  
 [How to Create Schemas for XML Messages](../core/how-to-create-schemas-for-xml-messages.md)   
 [Creating Schemas Using BizTalk Editor](../core/creating-schemas-using-biztalk-editor.md)