---
title: IDebugProperty2::GetDerivedMostProperty |Microsoft 文档
ms.custom: ''
ms.date: 11/04/2016
ms.technology:
- vs-ide-sdk
ms.topic: conceptual
f1_keywords:
- IDebugProperty2::GetDerivedMostProperty
helpviewer_keywords:
- IDebugProperty2::GetDerivedMostProperty
ms.assetid: cc86b461-62d1-4340-8209-c65037fd8b02
author: gregvanl
ms.author: gregvanl
manager: douge
ms.workload:
- vssdk
ms.openlocfilehash: f453dacf988b80cf6837b3324a9d4b0a70e2254e
ms.sourcegitcommit: 6a9d5bd75e50947659fd6c837111a6a547884e2a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2018
ms.locfileid: "31116703"
---
# <a name="idebugproperty2getderivedmostproperty"></a>IDebugProperty2::GetDerivedMostProperty
获取属性的派生程度最大属性。  
  
## <a name="syntax"></a>语法  
  
```cpp  
HRESULT GetDerivedMostProperty (   
   IDebugProperty2** ppDerivedMost  
);  
```  
  
```csharp  
int GetDerivedMostProperty (   
   out IDebugProperty2 ppDerivedMost  
);  
```  
  
#### <a name="parameters"></a>参数  
 `ppDerivedMost`  
 [out]返回[IDebugProperty2](../../../extensibility/debugger/reference/idebugproperty2.md)表示派生程度最大属性的对象。  
  
## <a name="return-value"></a>返回值  
 如果成功，则返回`S_OK`; 否则返回错误代码。 返回`S_GETDERIVEDMOST_NO_DERIVED_MOST`如果没有要检索的派生程度最大属性。  
  
## <a name="remarks"></a>备注  
 例如，如果此属性描述实现的对象`ClassRoot`但这是实际的实例化`ClassDerived`、 派生自`ClassRoot`，则此方法返回[IDebugProperty2](../../../extensibility/debugger/reference/idebugproperty2.md)对象描述`ClassDerived`对象。  
  
## <a name="see-also"></a>另请参阅  
 [IDebugProperty2](../../../extensibility/debugger/reference/idebugproperty2.md)