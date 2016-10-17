---
title: "This inheritance causes circular dependencies between &lt;type1&gt; &#39;&lt;typename1&gt;&#39; and its nested &lt;type2&gt; &#39;&lt;typename2&gt;&#39;"
ms.custom: na
ms.date: 10/01/2016
ms.prod: visual-studio-dev14
ms.reviewer: na
ms.suite: na
ms.technology: 
  - devlang-csharp
ms.tgt_pltfrm: na
ms.topic: article
ms.assetid: 17d4f938-5895-4d33-943e-8abf0ceacdc9
caps.latest.revision: 9
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
# This inheritance causes circular dependencies between &lt;type1&gt; &#39;&lt;typename1&gt;&#39; and its nested &lt;type2&gt; &#39;&lt;typename2&gt;&#39;
An inheritance structure results in circular dependency among nested classes, that is, two classes inheriting from each other.  
  
 The following code can generate this error message.  
  
```  
Public Class c1  
    Inherits c3.c4  
    Public Class c2  
    End Class  
End Class  
Public Class c3  
    Inherits c1.c2  
    Public Class c4  
    End Class  
End Class  
```  
  
 In the preceding code, class `c1` inherits from class `c4`, but `c4` is nested inside `c3`, which inherits from `c2`, nested inside `c1`.  
  
 **Error ID:** BC30907  
  
### To correct this error  
  
-   Change the inheritance structure so that there is no circular dependency.  
  
## See Also  
 [Inheritance Basics](../Topic/Inheritance%20Basics%20\(Visual%20Basic\).md)