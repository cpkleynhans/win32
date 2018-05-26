---
title: RB\_BEGINDRAG message
description: Puts the rebar control in drag-and-drop mode. This message does not cause a RBN\_BEGINDRAG notification to be sent.
ms.assetid: 1e3e4928-cb84-4fd4-8056-84de1f791d1c
keywords:
- RB_BEGINDRAG message Windows Controls
topic_type:
- apiref
api_name:
- RB_BEGINDRAG
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

# RB\_BEGINDRAG message

Puts the rebar control in drag-and-drop mode. This message does not cause a [RBN\_BEGINDRAG](rbn-begindrag.md) notification to be sent.

## Parameters

<dl> <dt>

*wParam* 
</dt> <dd>

Zero-based index of the band that the drag-and-drop operation will affect.

</dd> <dt>

*lParam* 
</dt> <dd>

**DWORD** value that contains the starting mouse coordinates. The horizontal coordinate is contained in the LOWORD and the vertical coordinate is contained in the HIWORD. If you pass (**DWORD**)-1, the rebar control will use the position of the mouse the last time the control's thread called [**GetMessage**](https://msdn.microsoft.com/library/windows/desktop/ms644936) or [**PeekMessage**](https://msdn.microsoft.com/library/windows/desktop/ms644943).

</dd> </dl>

## Return value

The return value for this message is not used.

## Remarks

The **RB\_BEGINDRAG**, [**RB\_DRAGMOVE**](rb-dragmove.md), and [**RB\_ENDDRAG**](rb-enddrag.md) messages allow you to implement an [**IDropTarget**](https://msdn.microsoft.com/library/windows/desktop/ms679679) interface for a rebar control. You send the **RB\_BEGINDRAG** message in response to [**IDropTarget::DragEnter**](https://msdn.microsoft.com/library/windows/desktop/ms680106), send the **RB\_DRAGMOVE** message in response to [**IDropTarget::DragOver**](https://msdn.microsoft.com/library/windows/desktop/ms680129), and the **RB\_ENDDRAG** message in response to [**IDropTarget::Drop**](https://msdn.microsoft.com/library/windows/desktop/ms687242) and [**IDropTarget::DragLeave**](https://msdn.microsoft.com/library/windows/desktop/ms680110).

## Requirements



|                                     |                                                                                       |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows Vista \[desktop apps only\]<br/>                                        |
| Minimum supported server<br/> | Windows Server 2003 \[desktop apps only\]<br/>                                  |
| Header<br/>                   | <dl> <dt>Commctrl.h</dt> </dl> |



 

 




