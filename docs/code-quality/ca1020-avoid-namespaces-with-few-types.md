---
title: CA1020：避免使用类型极少的命名空间
ms.date: 11/04/2016
ms.prod: visual-studio-dev15
ms.technology: vs-ide-code-analysis
ms.topic: reference
f1_keywords:
- CA1020
- AvoidNamespacesWithFewTypes
helpviewer_keywords:
- CA1020
- AvoidNamespacesWithFewTypes
ms.assetid: 9cb272f6-a3ff-45af-b35d-70dea620b074
author: gewarren
ms.author: gewarren
manager: douge
ms.workload:
- multiple
ms.openlocfilehash: d95e626349296f9b6c857263a78ce67751b471b5
ms.sourcegitcommit: 5b767247b3d819a99deb0dbce729a0562b9654ba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/20/2018
ms.locfileid: "39178925"
---
# <a name="ca1020-avoid-namespaces-with-few-types"></a>CA1020：避免使用类型极少的命名空间

|||
|-|-|
|TypeName|AvoidNamespacesWithFewTypes|
|CheckId|CA1020|
|类别|Microsoft.Design|
|是否重大更改|重大|

## <a name="cause"></a>原因

全局命名空间之外的命名空间包含少于五种类型。

## <a name="rule-description"></a>规则说明

请确保每个命名空间都有一个逻辑组织，并且存在正当理由将稀疏填充的命名空间中的类型。 命名空间应包含在大多数方案中一起使用的类型。 当其应用程序互相排斥，类型应位于单独的命名空间。 例如，<xref:System.Web.UI>命名空间包含 web 应用程序中使用的类型和<xref:System.Windows.Forms>命名空间包含类型中使用[!INCLUDE[TLA#tla_mswin](../code-quality/includes/tlasharptla_mswin_md.md)]-基于应用程序。 即使两个命名空间都具有控制用户界面各方面的类型，这些类型也并不是旨在用于同一应用程序。 因此，它们位于单独的命名空间中。 谨慎组织命名空间也会有所帮助，因为它增加了一项功能的可发现性。 通过检查命名空间层次结构，应该能够找到实现功能的类型库的使用者。

> [!NOTE]
> 设计时类型和权限不应合并到其他命名空间来遵守此原则。 这些类型位于下主命名空间，自己命名空间和命名空间应以结尾`.Design`和`.Permissions`分别。

## <a name="how-to-fix-violations"></a>如何解决冲突

若要修复此规则的冲突，请尝试将合并到单个命名空间包含几个类型的命名空间。

## <a name="when-to-suppress-warnings"></a>何时禁止显示警告

它可以安全地禁止显示此规则的警告时命名空间不包含与其他命名空间中的类型一起使用的类型。