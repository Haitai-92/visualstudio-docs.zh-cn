---
title: MSBuild 特殊字符 | Microsoft Docs
ms.custom: ''
ms.date: 11/04/2016
ms.technology: msbuild
ms.topic: conceptual
helpviewer_keywords:
- escape characters
- escape
- MSBuild Escape Characters
ms.assetid: 545e6a59-1093-4514-935e-78679a46fb3c
author: mikejo5000
ms.author: mikejo
manager: douge
ms.workload:
- multiple
ms.openlocfilehash: aa1e52e61f4003a9495e1bff5bd64e4edc40a323
ms.sourcegitcommit: 8ee7efb70a1bfebcb6dd9855b926a4ff043ecf35
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/17/2018
ms.locfileid: "39078649"
---
# <a name="msbuild-special-characters"></a>MSBuild 特殊字符
[!INCLUDE[vstecmsbuild](../extensibility/internals/includes/vstecmsbuild_md.md)] 保留一些专供在特定上下文中使用的字符。 如果要在保留此类字符的上下文中按原义使用这些字符，只能对这些字符进行转义。 例如，只有在项定义的 `Include` 和 `Exclude` 特性，以及对 `CreateItem` 的调用中，星号才具有特殊含义。 如果要让星号在上述某个上下文中显示为星号，必须进行转义。 在其他所有上下文中，只需在要显示星号的位置键入星号即可。  
  
 要转义特殊字符，请使用语法 %\<xx>，其中 \<xx> 表示字符的 ASCII 十六进制值。 有关详细信息，请参阅[如何：对 MSBuild 中的特殊字符进行转义](../msbuild/how-to-escape-special-characters-in-msbuild.md)。  
  
## <a name="special-characters"></a>特殊字符  
 下表列出了 [!INCLUDE[vstecmsbuild](../extensibility/internals/includes/vstecmsbuild_md.md)] 特殊字符：  
  
|字符|ASCII|**保留用法**|  
|-------------------|---------------|------------------------|  
|%|%25|引用元数据|  
|$|%24|引用属性|  
|@|%40|引用项列表|  
|'|%27|条件和其他表达式|  
|;|%3B|列表分隔符|  
|?|%3F|用于 `Include` 和 `Exclude` 特性中的文件名的通配符|  
|*|%2A|用于 `Include` 和 `Exclude` 特性中的文件名的通配符|  
  
## <a name="see-also"></a>请参阅  
 [高级概念](../msbuild/msbuild-advanced-concepts.md)   
 [项](../msbuild/msbuild-items.md)