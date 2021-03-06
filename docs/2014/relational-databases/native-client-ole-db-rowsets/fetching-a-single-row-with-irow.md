---
title: "Fetching a Single Row with IRow | Microsoft Docs"
ms.custom: ""
ms.date: "03/06/2017"
ms.prod: "sql-server-2014"
ms.reviewer: ""
ms.suite: ""
ms.technology: 
  - "database-engine"
  - "docset-sql-devref"
ms.tgt_pltfrm: ""
ms.topic: "reference"
helpviewer_keywords: 
  - "fetching rows"
  - "IRow interface"
  - "single row fetching [SQL Server Native Client]"
  - "OLE DB rowsets, fetching"
  - "rowsets [OLE DB], fetching"
  - "SQL Server Native Client OLE DB provider, fetching"
ms.assetid: 07c803ca-299a-42c5-ba02-360b9631d15f
caps.latest.revision: 30
author: "JennieHubbard"
ms.author: "jhubbard"
manager: "jhubbard"
---
# Fetching a Single Row with IRow
  The **IRow** interface implementation in the [!INCLUDE[ssNoVersion](../../includes/ssnoversion-md.md)] Native Client OLE DB provider is simplified to increase performance. **IRow** allows direct access to columns of a single row object. If you know beforehand that the result of a command execution will produce exactly one row, **IRow** will retrieve the columns of that row. If the result set includes multiple rows, **IRow** will expose only the first row.  
  
 The **IRow** implementation does not allow any navigation of the row. Each column in the row is accessed only one time with one exception: A column can be accessed one time to find the column size and again to fetch the data.  
  
> [!NOTE]  
>  **IRow::Open** supports only DBGUID_STREAM and DBGUID_NULL type of objects to be opened.  
  
 To obtain a row object using **ICommand::Execute** method, IID_IRow must be passed. The **IMultipleResults** interface must be used to handle multiple result sets. **IMultipleResults** supports **IRow** and **IRowset**. **IRowset** is used for bulk operations.  
  
## In This Section  
  
-   [Using IRow::GetColumns](using-irow-getcolumns.md)  
  
-   [Fetching BLOB Data Using IRow](../../database-engine/dev-guide/fetching-blob-data-using-irow.md)  
  
## See Also  
 [Rowsets](rowsets.md)  
  
  