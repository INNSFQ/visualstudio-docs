---
title: "How to: Target the Office multilingual user interface"
description: Learn how you can use Visual Studio to programmatically target the Microsoft Office multilingual user interface.
ms.custom: SEO-VS-2020
ms.date: "02/02/2017"
ms.topic: "how-to"
dev_langs:
  - "VB"
  - "CSharp"
helpviewer_keywords:
  - "globalization [Office development in Visual Studio], user interface targeting"
  - "MUI [Office development in Visual Studio]"
  - "Office applications [Office development in Visual Studio], localization"
  - "Multilingual User Interface [Office development in Visual Studio]"
  - "localization [Office development in Visual Studio], user interface targeting"
  - "Office applications [Office development in Visual Studio], globalization"
author: John-Hart
ms.author: johnhart
manager: jmartens
ms.technology: office-development
ms.workload:
  - "office"
---
# How to: Target the Office multilingual user interface

 [!INCLUDE [Visual Studio](~/includes/applies-to-version/vs-windows-only.md)]
  The Multilingual User Interface (MUI) is a Microsoft Office feature that gives the end user the ability to change the language of the user interface (UI). For example, an end user working with an English UI can change the language of the UI to Spanish.

 [!INCLUDE[appliesto_all](../vsto/includes/appliesto-all-md.md)]

 If your application will be used by people who use many languages of Office, you can add code to automatically change the language of your UI strings to match the language being used by Office on the user's computer (if the user has the correct resources installed).

## To check the current Office UI setting

1. Use the <xref:System.Threading.Thread.CurrentUICulture%2A> property of the current thread. Set the language of your UI strings to match the language used by the version of Office that currently runs on the user's computer.

     :::code language="vb" source="../vsto/codesnippet/VisualBasic/Trin_VstcoreCreatingExcelVB/Sheet1.vb" id="Snippet10":::
     :::code language="csharp" source="../vsto/codesnippet/CSharp/Trin_VstcoreCreatingExcelCS/Sheet1.cs" id="Snippet10":::

## See also
- [How to: Target Office applications through primary interop assemblies](../vsto/how-to-target-office-applications-through-primary-interop-assemblies.md)
- [Late binding in Office solutions](../vsto/late-binding-in-office-solutions.md)
