---
title: "&#39;ByRef&#39; parameter &#39;&lt;parametername&gt;&#39; cannot be used in a lambda expression"
ms.custom: na
ms.date: 10/01/2016
ms.prod: visual-studio-dev14
ms.reviewer: na
ms.suite: na
ms.technology: 
  - devlang-csharp
ms.tgt_pltfrm: na
ms.topic: article
ms.assetid: 5913f9b6-2929-4c05-8dd1-00b10fcd5a83
caps.latest.revision: 7
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
# &#39;ByRef&#39; parameter &#39;&lt;parametername&gt;&#39; cannot be used in a lambda expression
A lambda expression declared within a `Sub` or function cannot use any `ByRef` parameters of that `Sub` or function. For example, the following code will cause this error because the `ByRef` parameter `n` is used in the lambda expression.  
  
```  
'' Not valid.   
'Sub ExampleSub(ByRef n As Integer)  
  
'    Dim lambda = Function(p As Integer) p + n  
  
'End Sub  
```  
  
 **Error ID:** BC36639  
  
### To correct this error  
  
-   Assign the `ByRef` parameter to a local variable, and use the local variable in the lambda expression, as shown in the following code:  
  
    ```  
    Sub ExampleSub(ByRef n As Integer)  
  
        Dim temp = n  
        Dim lambda = Function(p As Integer) p + temp  
  
    End Sub  
    ```  
  
## See Also  
 [Lambda Expressions](../Topic/Lambda%20Expressions%20\(Visual%20Basic\).md)