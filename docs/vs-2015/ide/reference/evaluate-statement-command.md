---
title: "Evaluate Statement Command | Microsoft Docs"
ms.custom: ""
ms.date: "2018-06-30"
ms.prod: "visual-studio-dev14"
ms.reviewer: ""
ms.suite: ""
ms.technology: 
  - "vs-ide-general"
ms.tgt_pltfrm: ""
ms.topic: "article"
f1_keywords: 
  - "debug.evaluatestatement"
helpviewer_keywords: 
  - "Debug.EvaluateStatement command"
  - "Evaluate Statement command"
ms.assetid: 032039bc-9477-4f93-9b9d-66d4be0e90f4
caps.latest.revision: 19
author: gewarren
ms.author: gewarren
manager: "ghogen"
---
# Evaluate Statement Command
[!INCLUDE[vs2017banner](../../includes/vs2017banner.md)]

The latest version of this topic can be found at [Evaluate Statement Command](https://docs.microsoft.com/visualstudio/ide/reference/evaluate-statement-command).  
  
  
Evaluates and displays the given statement.  
  
## Syntax  
  
```  
Debug.EvaluateStatement text   
```  
  
## Arguments  
 `text`  
 Required. The statement to evaluate.  
  
## Remarks  
 The window used to enter the **EvaluateStatement** command determines whether an equals sign (=) is interpreted as a comparison operator or as an assignment operator.  
  
 In the **Command** window, an equals sign (=) is interpreted as a comparison operator. So, for example, if the values of variables `a` and `b` are different, then the command  
  
```  
>Debug.EvaluateStatement(a=b)  
```  
  
 will return a value of `false`.  
  
 In the **Immediate** window, by contrast, an equals sign (=) is interpreted as an assignment operator. So, for example, the command  
  
```  
>Debug.EvaluateStatement(a=b)  
```  
  
 will assign to variable `a` the value of variable `b`.  
  
## Example  
  
```  
>Debug.EvaluateStatement(a+b)  
```  
  
## See Also  
 [Print Command](../../ide/reference/print-command.md)   
 [Visual Studio Commands](../../ide/reference/visual-studio-commands.md)   
 [Command Window](../../ide/reference/command-window.md)   
 [Find/Command Box](../../ide/find-command-box.md)   
 [Visual Studio Command Aliases](../../ide/reference/visual-studio-command-aliases.md)


