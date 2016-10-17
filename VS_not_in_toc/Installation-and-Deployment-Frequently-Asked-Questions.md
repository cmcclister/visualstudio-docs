---
title: "Installation and Deployment Frequently Asked Questions"
ms.custom: na
ms.date: 10/01/2016
ms.prod: visual-studio-dev14
ms.reviewer: na
ms.suite: na
ms.technology: 
  - devlang-csharp
ms.tgt_pltfrm: na
ms.topic: article
ms.assetid: 4ac62bf3-e335-4899-9074-89bcd004dc65
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
# Installation and Deployment Frequently Asked Questions
This topic addresses questions from the Visual Studio SDK user community about installation and deployment. The topic will continue to be updated with new content from the community.  
  
## Contents  
  
-   [Determining the LCID of a Visual Studio Installation Programmatically](#DeterminingtheLCIDofaVisualStudioInstallationProgrammatically)  
  
##  <a name="DeterminingtheLCIDofaVisualStudioInstallationProgrammatically"></a> Determining the LCID of a Visual Studio Installation Programmatically  
 **Q:** Is there a way to programmatically determine the LCID of a Visual Studio installation?  
  
 **A:**  <xref:Microsoft.VisualStudio.Shell.Interop.IUIHostLocale2.GetUILocale?qualifyHint=False> or <xref:Microsoft.VisualStudio.Shell.Interop.IUIHostLocale.GetUILocale?qualifyHint=False>will return the LCID of Visual Studio currently in use.  
  
## See Also  
 [Releasing a Product](../VS_not_in_toc/Releasing-a-Visual-Studio-Integration-Product.md)