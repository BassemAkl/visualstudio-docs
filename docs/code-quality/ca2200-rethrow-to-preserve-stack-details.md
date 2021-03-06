---
title: "CA2200: Rethrow to preserve stack details | Microsoft Docs"
ms.custom: ""
ms.date: "11/04/2016"
ms.reviewer: ""
ms.suite: ""
ms.technology: 
  - "vs-devops-test"
ms.tgt_pltfrm: ""
ms.topic: "article"
f1_keywords: 
  - "RethrowToPreserveStackDetails"
  - "CA2200"
helpviewer_keywords: 
  - "CA2200"
  - "RethrowToPreserveStackDetails"
ms.assetid: 046e1b98-c4dc-4515-874f-9c0de2285621
caps.latest.revision: 13
author: "gewarren"
ms.author: "gewarren"
manager: "ghogen"
translation.priority.ht: 
  - "cs-cz"
  - "de-de"
  - "es-es"
  - "fr-fr"
  - "it-it"
  - "ja-jp"
  - "ko-kr"
  - "pl-pl"
  - "pt-br"
  - "ru-ru"
  - "tr-tr"
  - "zh-cn"
  - "zh-tw"
---
# CA2200: Rethrow to preserve stack details
|||  
|-|-|  
|TypeName|RethrowToPreserveStackDetails|  
|CheckId|CA2200|  
|Category|Microsoft.Usage|  
|Breaking Change|Non Breaking|  
  
## Cause  
 An exception is re-thrown and the exception is explicitly specified in the `throw` statement.  
  
## Rule Description  
 Once an exception is thrown, part of the information it carries is the stack trace. The stack trace is a list of the method call hierarchy that starts with the method that throws the exception and ends with the method that catches the exception. If an exception is re-thrown by specifying the exception in the `throw` statement, the stack trace is restarted at the current method and the list of method calls between the original method that threw the exception and the current method is lost. To keep the original stack trace information with the exception, use the `throw` statement without specifying the exception.  
  
## How to Fix Violations  
 To fix a violation of this rule, re-throw the exception without specifying the exception explicitly.  
  
## When to Suppress Warnings  
 Do not suppress a warning from this rule.  
  
## Example  
 The following example shows a method, `CatchAndRethrowExplicitly`, which violates the rule and a method, `CatchAndRethrowImplicitly`, which satisfies the rule.  
  
 [!code-csharp[FxCop.Usage.Rethrow#1](../code-quality/codesnippet/CSharp/ca2200-rethrow-to-preserve-stack-details_1.cs)]
 [!code-vb[FxCop.Usage.Rethrow#1](../code-quality/codesnippet/VisualBasic/ca2200-rethrow-to-preserve-stack-details_1.vb)]