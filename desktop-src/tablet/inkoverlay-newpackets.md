---
Description: Occurs when the ink collecto rreceives a packet.
ms.assetid: 26d5a3eb-430a-4e21-8a3f-fdec5005cd6e
title: InkOverlay.NewPackets event
ms.date: 05/31/2018
ms.topic: article
ms.author: windowssdkdev
ms.prod: windows
ms.technology: desktop
---

# InkOverlay.NewPackets event

Occurs when the ink collecto rreceives a packet

## Syntax


```C++
void NewPackets(
  [in]      IInkCursor     *Cursor,
  [in]      IInkStrokeDisp *Stroke,
  [in]      long           PacketCount,
  [in, out] VARIANT        *PacketData
);
```



## Parameters

<dl> <dt>

*Cursor* \[in\]
</dt> <dd>

The [**IInkCursor**](/windows/win32/msinkaut/nn-msinkaut-iinkcursor?branch=master) object that generated the [**NewInAirPackets**](inkcollector-newinairpackets.md) event.

</dd> <dt>

*Stroke* \[in\]
</dt> <dd>

Specifies the [**IInkStrokeDisp**](/windows/win32/msinkaut/nn-msinkaut-iinkstrokedisp?branch=master) object.

</dd> <dt>

*PacketCount* \[in\]
</dt> <dd>

The number of packets received for a [**IInkStrokeDisp**](/windows/win32/msinkaut/nn-msinkaut-iinkstrokedisp?branch=master) object.

</dd> <dt>

*PacketData* \[in, out\]
</dt> <dd>

An array that contains the selected data for the packet.

For more information about the VARIANT structure, see [Using the COM Library](using-the-com-library.md).

</dd> </dl>

## Return value

This event does not return a value.

## Remarks

Packets are received while a stroke is being collected. Packet events occur rapidly, and a [**NewPackets**](inkcollector-newpackets.md) event handler must be fast or performance suffers.

This event method is defined in the \_IInkCollectorEvents, \_IInkOverlayEvents, and \_IInkPictureEvents dispatch-only interfaces (dispinterfaces) with an ID of DISPID\_ICENewPackets.

This event should be used carefully as it could have an adverse effect on ink performance if too much code is executed in the event handlers.

To set which properties are contained in this array, use the [**DesiredPacketDescription**](/windows/win32/msinkaut/?branch=master) property of the ink collector object. The array that the *PacketData* parameter returns contains the data for those properties.

> [!Note]  
> Although you can modify the packet data, these modifications are not persisted or used.

 

## Requirements



|                                     |                                                                                                                     |
|-------------------------------------|---------------------------------------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows XP Tablet PC Edition \[desktop apps only\]<br/>                                                       |
| Minimum supported server<br/> | None supported<br/>                                                                                           |
| Header<br/>                   | <dl> <dt>Msinkaut.h (also requires Msinkaut\_i.c)</dt> </dl> |
| Library<br/>                  | <dl> <dt>InkObj.dll</dt> </dl>                               |



## See also

<dl> <dt>

[**InkOverlay Class**](/windows/win32/msinkaut/?branch=master)
</dt> <dt>

[**NewInAirPackets Event**](inkcollector-newinairpackets.md)
</dt> <dt>

[**IInkCursor Interface**](/windows/win32/msinkaut/nn-msinkaut-iinkcursor?branch=master)
</dt> <dt>

[**IInkStrokeDisp Interface**](/windows/win32/msinkaut/nn-msinkaut-iinkstrokedisp?branch=master)
</dt> </dl>

 

 



