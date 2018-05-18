﻿---
Description: 'This section describes the system-supplied FilterXxx functions that user-mode applications can use to communicate with kernel-mode file system minifilter drivers.'
ms.assetid: '6e4d6aea-9498-49cf-b3ed-ea3d9467c65e'
title: 'Minifilter User-Mode Application Functions'
---

# Minifilter User-Mode Application Functions

This section describes the system-supplied **Filter***Xxx* functions that user-mode applications can use to communicate with kernel-mode file system minifilter drivers. The functions are in alphabetical order.

## 

## In this section



| Topic                                                                               | Description                                                                                                                                                                                                                                                                                                                                                 |
|-------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [**FilterAttach**](filterattach.md)<br/>                                     | The **FilterAttach** function attaches a new minifilter instance to the given volume. <br/>                                                                                                                                                                                                                                                           |
| [**FilterAttachAtAltitude**](filterattachataltitude.md)<br/>                 | The **FilterAttachAtAltitude** function is a debugging support function that attaches a new minifilter instance to a volume at a specified altitude, overriding any settings in the minifilter's setup information (INF) file. <br/>                                                                                                                  |
| [**FilterClose**](filterclose.md)<br/>                                       | The **FilterClose** function closes an open minifilter handle. <br/>                                                                                                                                                                                                                                                                                  |
| [**FilterConnectCommunicationPort**](filterconnectcommunicationport.md)<br/> | **FilterConnectCommunicationPort** opens a new connection to a communication server port that is created by a file system minifilter. <br/>                                                                                                                                                                                                           |
| [**FilterCreate**](filtercreate.md)<br/>                                     | The **FilterCreate** function creates a handle for the given minifilter. <br/>                                                                                                                                                                                                                                                                        |
| [**FilterDetach**](filterdetach.md)<br/>                                     | The **FilterDetach** function detaches the given minifilter instance from the given volume. <br/>                                                                                                                                                                                                                                                     |
| [**FilterFindClose**](filterfindclose.md)<br/>                               | The **FilterFindClose** function closes the specified minifilter search handle. The [**FilterFindFirst**](filterfindfirst.md) and [**FilterFindNext**](filterfindnext.md) functions use this search handle to locate minifilters. <br/>                                                                                                             |
| [**FilterFindFirst**](filterfindfirst.md)<br/>                               | The **FilterFindFirst** function returns information about a filter driver (minifilter driver instance or legacy filter driver) and is used to begin scanning the filters in the global list of registered filters.<br/>                                                                                                                              |
| [**FilterFindNext**](filterfindnext.md)<br/>                                 | The **FilterFindNext** function continues a filter search started by a call to [**FilterFindFirst**](filterfindfirst.md). <br/>                                                                                                                                                                                                                      |
| [**FilterGetDosName**](filtergetdosname.md)<br/>                             | The **FilterGetDosName** function returns the MS-DOS device name that corresponds to the given volume name. <br/>                                                                                                                                                                                                                                     |
| [**FilterGetInformation**](filtergetinformation.md)<br/>                     | The **FilterGetInformation** function returns various kinds of information about a minifilter.<br/>                                                                                                                                                                                                                                                   |
| [**FilterGetMessage**](filtergetmessage.md)<br/>                             | The **FilterGetMessage** function gets a message from a kernel-mode minifilter. <br/>                                                                                                                                                                                                                                                                 |
| [**FilterInstanceClose**](filterinstanceclose.md)<br/>                       | The **FilterInstanceClose** function closes a minifilter instance handle opened by **FilterInstanceCreate**. <br/>                                                                                                                                                                                                                                    |
| [**FilterInstanceCreate**](filterinstancecreate.md)<br/>                     | The **FilterInstanceCreate** function creates a handle that can be used to communicate with the given minifilter instance. <br/>                                                                                                                                                                                                                      |
| [**FilterInstanceFindClose**](filterinstancefindclose.md)<br/>               | The **FilterInstanceFindClose** function closes the specified minifilter instance search handle. The [**FilterInstanceFindFirst**](filterinstancefindfirst.md) and [**FilterInstanceFindNext**](filterinstancefindnext.md) functions use this search handle to locate instances of a minifilter. <br/>                                              |
| [**FilterInstanceFindFirst**](filterinstancefindfirst.md)<br/>               | The **FilterInstanceFindFirst** function returns information about a minifilter driver instance and is used as a starting point for scanning the instances of a minifilter. <br/>                                                                                                                                                                     |
| [**FilterInstanceFindNext**](filterinstancefindnext.md)<br/>                 | The **FilterInstanceFindNext** function continues a minifilter driver instance search started by a call to [**FilterInstanceFindFirst**](filterinstancefindfirst.md). <br/>                                                                                                                                                                          |
| [**FilterInstanceGetInformation**](filterinstancegetinformation.md)<br/>     | The **FilterInstanceGetInformation** function returns various kinds of information about a minifilter instance. <br/>                                                                                                                                                                                                                                 |
| [**FilterLoad**](filterload.md)<br/>                                         | The **FilterLoad** function dynamically loads a minifilter driver into the system. <br/>                                                                                                                                                                                                                                                              |
| [**FilterReplyMessage**](filterreplymessage.md)<br/>                         | The **FilterReplyMessage** function replies to a message from a kernel-mode minifilter. <br/>                                                                                                                                                                                                                                                         |
| [**FilterSendMessage**](filtersendmessage.md)<br/>                           | The **FilterSendMessage** function sends a message to a kernel-mode minifilter. <br/>                                                                                                                                                                                                                                                                 |
| [**FilterUnload**](filterunload.md)<br/>                                     | An application that has loaded a supporting minifilter by calling [**FilterLoad**](filterload.md) can unload the minifilter by calling the **FilterUnload** function. <br/>                                                                                                                                                                          |
| [**FilterVolumeFindClose**](filtervolumefindclose.md)<br/>                   | The **FilterVolumeFindClose** function closes the specified volume search handle. [**FilterVolumeFindFirst**](filtervolumefindfirst.md) and [**FilterVolumeFindNext**](filtervolumefindnext.md) use this search handle to locate volumes. <br/>                                                                                                     |
| [**FilterVolumeFindFirst**](filtervolumefindfirst.md)<br/>                   | The **FilterVolumeFindFirst** function returns information about a volume.<br/>                                                                                                                                                                                                                                                                       |
| [**FilterVolumeFindNext**](filtervolumefindnext.md)<br/>                     | The **FilterVolumeFindNext** function continues a volume search started by a call to [**FilterVolumeFindFirst**](filtervolumefindfirst.md).<br/>                                                                                                                                                                                                     |
| [**FilterVolumeInstanceFindClose**](filtervolumeinstancefindclose.md)<br/>   | The [**FilterVolumeInstanceFindClose**](filtervolumeinstancefindclose.md) function closes the specified volume instance search handle. [**FilterVolumeInstanceFindFirst**](filtervolumeinstancefindfirst.md) and [**FilterVolumeInstanceFindNext**](filtervolumeinstancefindnext.md) use this search handle to locate instances on a volume. <br/> |
| [**FilterVolumeInstanceFindFirst**](filtervolumeinstancefindfirst.md)<br/>   | The **FilterVolumeInstanceFindFirst** function returns information about a minifilter driver instance or legacy filter driver and is used to begin scanning the filter drivers that are attached to a volume.<br/>                                                                                                                                    |
| [**FilterVolumeInstanceFindNext**](filtervolumeinstancefindnext.md)<br/>     | The **FilterVolumeInstanceFindNext** function continues a minifilter driver instance or legacy filter driver search started by a call to [**FilterVolumeInstanceFindFirst**](filtervolumeinstancefindfirst.md). <br/>                                                                                                                                |



 

## Related topics

<dl> <dt>

[Installable file systems driver design guide](http://go.microsoft.com/fwlink/p/?LinkId=798410)
</dt> </dl>

 

 

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20%5Bifsk\ifsk%5D:%20Minifilter%20User-Mode%20Application%20Functions%20%20RELEASE:%20%283/30/2018%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/en-us/default.aspx. "Send comments about this topic to Microsoft")




