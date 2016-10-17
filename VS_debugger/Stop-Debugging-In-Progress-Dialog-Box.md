---
title: "Stop Debugging In Progress Dialog Box"
ms.custom: na
ms.date: 10/03/2016
ms.devlang: 
  - FSharp
  - VB
  - CSharp
  - C++
  - JScript
  - SQL
  - VB
  - CSharp
  - C++
ms.prod: visual-studio-dev14
ms.reviewer: na
ms.suite: na
ms.technology: 
  - vs-ide-debug
ms.tgt_pltfrm: na
ms.topic: article
ms.assetid: ed7ef49d-e25f-4a4d-9396-9bc7b4143117
caps.latest.revision: 7
manager: ghogen
translation.priority.ht: 
  - cs-cz
  - de-de
  - es-es
  - fr-fr
  - it-it
  - ja-jp
  - ko-kr
  - pl-pl
  - pt-br
  - ru-ru
  - tr-tr
  - zh-cn
  - zh-tw
---
# Stop Debugging In Progress Dialog Box
This dialog box appears when the debugger is trying to stop a debugging session, but stopping the session is going to take some time. Stopping a debugging session is normally very fast and this dialog box does not appear. Sometimes, however, it takes additional time to detach from all the processes being debugged. If stopping the session takes more than a few seconds (or if a detach error occurs), this dialog box appears. If this occurs frequently, it may be due to an internal problem and you may want to contact Product Support Services.  
  
 You can wait for the processes to detach and this dialog box to disappear, or use the **Stop Now** button to force immediate termination.  
  
 **Stop Now**  
 Click this button to end the debugging session immediately. Using **Stop Now**will terminate rather than detaching the processes being debugged. If you are debugging system processes, terminating those processes with **Stop Now** can have unexpected and undesired effects.  
  
## See Also  
 [Debugger Security](../VS_debugger/Debugger-Security.md)   
 [Detaching Programs](assetId:///f2c756c2-8079-474b-94c2-01c19a141a01)