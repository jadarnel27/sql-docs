---
title: "Connect to an Oracle Database (SSAS) | Microsoft Docs"
ms.custom: ""
ms.date: "06/13/2017"
ms.prod: "sql-server-2014"
ms.reviewer: ""
ms.suite: ""
ms.technology: 
  - "analysis-services"
ms.tgt_pltfrm: ""
ms.topic: "article"
f1_keywords: 
  - "sql12.asvs.bidtoolset.connoracledb.f1"
ms.assetid: 9bd177fb-8539-46cd-bf96-189ade52c2a1
caps.latest.revision: 10
author: "Minewiskan"
ms.author: "owend"
manager: "mblythe"
---
# Connect to an Oracle Database (SSAS)
  This page of the **Table Import Wizard** enables you to specify settings to connect to an Oracle database. To access the wizard from the [!INCLUDE[ssBIDevStudio](../includes/ssbidevstudio-md.md)], on the **Model** menu, click **Import from Data Source**.  
  
 To connect to a data source, you must have the appropriate provider installed on your computer.  
  
> [!NOTE]  
>  The credentials of the current user are used when selecting a database in this page. However, import will not succeed if the user specified in the Impersonation Information page does not have sufficient privileges to read from the selected database.  
  
## UIElement List  
 **Friendly connection name**  
 Type a unique name for this data source connection. This is a required field.  
  
 **Server name**  
 Type or select the name of the server instance to connect to.  
  
 **User name**  
 Specify a user name for the database connection.  
  
 This user name is used when constructing the connection string for the data source. These credentials are also used when previewing and filtering data in the Table Properties window and in the Import Wizard. These credentials are not used to import or refresh data; the Windows credentials specified on the Impersonation Information page are used instead.  
  
 **Password**  
 Specify a password for the database connection.  
  
 **Save my password**  
 Specify whether the password you have entered in the **Password** box is stored.  
  
 **Advanced**  
 Set additional connection properties by using the **Set Advanced Properties** dialog box. For more information, see [Set Advanced Properties &#40;SSAS&#41;](set-advanced-properties-ssas.md).  
  
 **Test Connection**  
 Attempt to establish a connection to the data source using the current settings. A message is displayed indicating whether the connection is successful.  
  
  