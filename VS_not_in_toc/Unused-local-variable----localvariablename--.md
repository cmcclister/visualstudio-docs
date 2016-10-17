---
title: "Unused local variable: &#39;&lt;localvariablename&gt;&#39;"
ms.custom: na
ms.date: 10/01/2016
ms.prod: visual-studio-dev14
ms.reviewer: na
ms.suite: na
ms.technology: 
  - devlang-csharp
ms.tgt_pltfrm: na
ms.topic: article
ms.assetid: 749b1315-0f85-4f7e-b68b-8cc4346c502b
caps.latest.revision: 10
manager: douge
translation.priority.ht: 
  - de-de
  - es-es
  - fr-fr
  - it-it
  - ja-jp
  - ko-kr
  - ru-ru
  - zh-cn
  - zh-tw
translation.priority.mt: 
  - cs-cz
  - pl-pl
  - pt-br
  - tr-tr
---
# Unused local variable: &#39;&lt;localvariablename&gt;&#39;
A local variable in a procedure is declared but never used.  
  
 One possibility is that there is a spelling mistake among the local variables in the procedure. If this variable is in fact used in another statement but spelled differently, it will appear to the compiler as two different variables.  
  
 By default, this message is a warning. For more information about hiding warnings or treating warnings as errors, see [Configuring Warnings in Visual Basic](../VS_IDE/Configuring-Warnings-in-Visual-Basic.md).  
  
 **Error ID:** BC42024  
  
### To correct this error  
  
1.  Check for spelling mistakes among the local variables within the procedure. Notice that casing does not make a difference. The names `ABC` and `abc` are considered to refer to the same variable.  
  
2.  If there is no spelling mistake, either remove the declaration of this variable or use it in another statement in the procedure.  
  
## See Also  
 [Declared Element Names](../Topic/Declared%20Element%20Names%20\(Visual%20Basic\).md)   
 [Dim Statement](../Topic/Dim%20Statement%20\(Visual%20Basic\).md)