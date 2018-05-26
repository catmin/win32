---
title: TCM\_GETROWCOUNT message
description: Retrieves the current number of rows of tabs in a tab control. You can send this message explicitly or by using the TabCtrl\_GetRowCount macro.
ms.assetid: ef104374-1030-46c3-876e-083df73854ab
keywords:
- TCM_GETROWCOUNT message Windows Controls
topic_type:
- apiref
api_name:
- TCM_GETROWCOUNT
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

# TCM\_GETROWCOUNT message

Retrieves the current number of rows of tabs in a tab control. You can send this message explicitly or by using the [**TabCtrl\_GetRowCount**](/windows/win32/Commctrl/nf-commctrl-tabctrl_getrowcount?branch=master) macro.

## Parameters

<dl> <dt>

*wParam* 
</dt> <dd>Must be zero.</dd> <dt>

*lParam* 
</dt> <dd>Must be zero.</dd> </dl>

## Return value

Returns the number of rows of tabs.

## Remarks

Only tab controls that have the [**TCS\_MULTILINE**](tab-control-styles.md#tcs-multiline) style can have multiple rows of tabs.

## Requirements



|                                     |                                                                                       |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows Vista \[desktop apps only\]<br/>                                        |
| Minimum supported server<br/> | Windows Server 2003 \[desktop apps only\]<br/>                                  |
| Header<br/>                   | <dl> <dt>Commctrl.h</dt> </dl> |



 

 




