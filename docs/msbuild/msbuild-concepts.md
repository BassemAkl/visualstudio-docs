---
title: "MSBuild Concepts | Microsoft Docs"
ms.custom: ""
ms.date: "11/04/2016"
ms.reviewer: ""
ms.suite: ""
ms.technology: 
  - "vs-ide-sdk"
ms.tgt_pltfrm: ""
ms.topic: "article"
helpviewer_keywords: 
  - "MSBuild, concepts"
ms.assetid: 083b8ba3-e4ad-45af-bb5d-3bc81d406131
caps.latest.revision: 13
author: "kempb"
ms.author: "kempb"
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
# MSBuild Concepts
[!INCLUDE[vstecmsbuild](../extensibility/internals/includes/vstecmsbuild_md.md)] provides a basic XML schema that you can use to control how the build platform builds software. To specify the components in the build and how they are to be built, use these four parts of MSBuild: properties, items, tasks, and targets.  
  
## Related Topics  
  
|Title|Description|  
|-----------|-----------------|  
|[MSBuild Properties](../msbuild/msbuild-properties.md)|Introduces properties and property collections. Properties are key/value pairs that you can use to configure builds.|  
|[Items](../msbuild/msbuild-items.md)|Describes the general concepts behind the [!INCLUDE[vstecmsbuild](../extensibility/internals/includes/vstecmsbuild_md.md)] file format and how the pieces fit together.|  
|[Targets](../msbuild/msbuild-targets.md)|Explains how to group tasks together in a particular order and enable sections of the build process to be called on the command line.|  
|[Tasks](../msbuild/msbuild-tasks.md)|Shows how to create a unit of executable code that can be used by [!INCLUDE[vstecmsbuild](../extensibility/internals/includes/vstecmsbuild_md.md)] to perform atomic build operations.|  
|[Comparing Properties and Items](../msbuild/comparing-properties-and-items.md)|Compares MSBuild properties and items. Both are used to pass information to tasks, evaluate conditions, and store values that can be referenced throughout the project file.|  
|[MSBuild Special Characters](../msbuild/msbuild-special-characters.md)|Explains how to escape some characters that [!INCLUDE[vstecmsbuild](../extensibility/internals/includes/vstecmsbuild_md.md)] reserves for special use in specific contexts.|  
|[Walkthrough: Creating an MSBuild Project File from Scratch](../msbuild/walkthrough-creating-an-msbuild-project-file-from-scratch.md)|Shows how to create a basic project file incrementally, by using only a text editor.|  
|[Walkthrough: Using MSBuild](../msbuild/walkthrough-using-msbuild.md)|Introduces the building blocks of MSBuild and shows how to write, manipulate, and debug MSBuild projects without closing the Visual Studio integrated development environment (IDE).|  
|[MSBuild Reference](../msbuild/msbuild-reference.md)|Links to documents that contain reference information.|  
|[MSBuild](../msbuild/msbuild.md)|Presents an overview of the XML schema for a project file and shows how it controls processes that builds software.|