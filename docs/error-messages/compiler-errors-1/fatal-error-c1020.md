---
title: "Fatal Error C1020 | Microsoft Docs"
ms.custom: ""
ms.date: "11/04/2016"
ms.reviewer: ""
ms.suite: ""
ms.technology: ["cpp-tools"]
ms.tgt_pltfrm: ""
ms.topic: "article"
f1_keywords: ["C1020"]
dev_langs: ["C++"]
helpviewer_keywords: ["C1020"]
ms.assetid: 42f429e2-5e3b-4086-a10d-b99e032e51c5
caps.latest.revision: 8
author: "corob-msft"
ms.author: "corob"
manager: "ghogen"
ms.workload: ["cplusplus"]
---
# Fatal Error C1020
unexpected #endif  
  
 The `#endif` directive has no matching `#if`, `#ifdef`, or `#ifndef` directive. Be sure each `#endif` has a matching directive.  
  
 The following sample generates C1020:  
  
```  
// C1020.cpp  
#endif     // C1020  
```  
  
 Possible resolution:  
  
```  
// C1020b.cpp  
// compile with: /c  
#if 1  
#endif  
```