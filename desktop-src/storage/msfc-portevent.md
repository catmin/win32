---
title: MSFC\_PortEvent structure
description: A WMI provider uses the MSFC\_PortEvent structure to report port events for the indicated adapter.
ms.assetid: 'bf9e2d58-9379-4b88-9043-580a97ec7cd9'
keywords: ["MSFC_PortEvent structure Storage Devices", "PMSFC_PortEvent structure pointer Storage Devices"]
topic_type:
- apiref
api_name:
- MSFC_PortEvent
api_location:
- hbapiwmi.h
api_type:
- HeaderDef
---

# MSFC\_PortEvent structure

A WMI provider uses the MSFC\_PortEvent structure to report port events for the indicated adapter.

## Syntax


```C++
typedef struct _MSFC_PortEvent {
  ULONG EventType;
  ULONG FabricPortId;
  UCHAR PortWWN[8];
} MSFC_PortEvent, *PMSFC_PortEvent;
```



## Members

<dl> <dt>

**EventType**
</dt> <dd>

Indicates the type of the event. The values that can be assigned to this member are defined by the [EVENT\_TYPE\_QUALIFIERS](https://msdn.microsoft.com/library/windows/hardware/ff553764) WMI class qualifier.

</dd> <dt>

**FabricPortId**
</dt> <dd>

Contains the fabric port ID.

</dd> <dt>

**PortWWN**
</dt> <dd>

Contains the worldwide name that indicates the port for which the event occurred.

</dd> </dl>

## Requirements



|                   |                                                                                                            |
|-------------------|------------------------------------------------------------------------------------------------------------|
| Header<br/> | <dl> <dt>Hbapiwmi.h (include Hbapiwmi.h)</dt> </dl> |



## See also

<dl> <dt>

[EVENT\_TYPE\_QUALIFIERS](https://msdn.microsoft.com/library/windows/hardware/ff553764)
</dt> </dl>

�

�

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20%5Bstorage\storage%5D:%20MSFC_PortEvent%20structure%20%20RELEASE:%20%283/29/2018%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/default.aspx. "Send comments about this topic to Microsoft")





