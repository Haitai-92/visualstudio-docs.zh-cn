---
title: IDebugProcess3::Continue |Microsoft 文档
ms.custom: ''
ms.date: 11/04/2016
ms.technology:
- vs-ide-sdk
ms.topic: conceptual
f1_keywords:
- IDebugProcess3::Continue
helpviewer_keywords:
- IDebugProcess3::Continue
ms.assetid: 57506242-5763-4c08-adb9-8a78ce02cebb
author: gregvanl
ms.author: gregvanl
manager: douge
ms.workload:
- vssdk
ms.openlocfilehash: 38bb11237d5016e3747c5a615e61144511c17fad
ms.sourcegitcommit: 6a9d5bd75e50947659fd6c837111a6a547884e2a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2018
ms.locfileid: "31117473"
---
# <a name="idebugprocess3continue"></a>IDebugProcess3::Continue
将继续运行此过程从已停止状态。 保留任何以前的执行状态 （如步骤），并再次执行的进程启动。  
  
> [!NOTE]
>  此方法应使用而不是[继续](../../../extensibility/debugger/reference/idebugprogram2-continue.md)。  
  
## <a name="syntax"></a>语法  
  
```cpp  
HRESULT Continue(  
   IDebugThread2* pThread  
);  
```  
  
```csharp  
int Continue(  
   IDebugThread2 pThread  
);  
```  
  
#### <a name="parameters"></a>参数  
 `pThread`  
 [in][IDebugThread2](../../../extensibility/debugger/reference/idebugthread2.md)对象表示要能继续的线程。  
  
## <a name="return-value"></a>返回值  
 如果成功，则返回`S_OK`; 否则为返回错误代码。  
  
## <a name="remarks"></a>备注  
 在此过程而不考虑多少进程正在调试，或哪个进程生成 stopping 事件上调用此方法。 实现必须保留以前的执行状态 （如步骤），并继续执行，就像它已完成其之前执行之前永远不会停止。 也就是说，如果中的线程则此过程将正在进行操作逐过程操作并且由于某些其他进程已停止，已停止，然后`Continue`调用，指定线程必须完成原始逐过程操作。  
  
 **警告**不发送 stopping 事件或即时 （同步） 事件与[事件](../../../extensibility/debugger/reference/idebugeventcallback2-event.md)时处理此调用; 否则调试器可能会挂起。  
  
## <a name="see-also"></a>另请参阅  
 [IDebugProcess3](../../../extensibility/debugger/reference/idebugprocess3.md)   
 [IDebugThread2](../../../extensibility/debugger/reference/idebugthread2.md)   
 [Event](../../../extensibility/debugger/reference/idebugeventcallback2-event.md)