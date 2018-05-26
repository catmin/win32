---
title: NM\_NCHITTEST (rebar) notification code
description: Sent by a rebar control when the control receives a WM\_NCHITTEST message. This notification code is sent in the form of a WM\_NOTIFY message.
ms.assetid: b345d83e-682d-4067-a783-689d64f9b7bc
keywords:
- NM_NCHITTEST (rebar) notification code Windows Controls
topic_type:
- apiref
api_name:
- NM_NCHITTEST
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.date: 05/31/2018
ms.topic: article
ms.author: windowssdkdev
ms.prod: windows
ms.technology: desktop
---

# NM\_NCHITTEST (rebar) notification code

Sent by a rebar control when the control receives a [**WM\_NCHITTEST**](https://msdn.microsoft.com/library/windows/desktop/ms645618) message. This notification code is sent in the form of a [**WM\_NOTIFY**](wm-notify.md) message.


```C++
NM_NCHITTEST

    lpnmmouse = (LPNMMOUSE) lParam;
```



## Parameters

<dl> <dt>

*lParam* 
</dt> <dd>

Pointer to an [**NMMOUSE**](/windows/win32/Commctrl/ns-commctrl-tagnmmouse?branch=master) structure that contains information about the notification code. The **dwItemSpec** member contains the band index over which the hit test message occurred, and the **pt** member contains the mouse coordinates of the hit test message.

</dd> </dl>

## Return value

Return zero to allow the rebar to perform default processing of the hit test message, or return one of the HT\* values documented under [**WM\_NCHITTEST**](https://msdn.microsoft.com/library/windows/desktop/ms645618) to override the default hit test processing.

## Requirements



|                                     |                                                                                       |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows Vista \[desktop apps only\]<br/>                                        |
| Minimum supported server<br/> | Windows Server 2003 \[desktop apps only\]<br/>                                  |
| Header<br/>                   | <dl> <dt>Commctrl.h</dt> </dl> |



 

 




