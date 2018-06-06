---
Description: Specifies the microphone array geometry for the Voice Capture DSP.
ms.assetid: 1d91bdc8-5a09-487d-b45e-80d57a44cd0e
title: MFPKEY\_WMAAECMA\_MICARRAY\_DESCPTR Property
ms.technology: desktop
ms.prod: windows
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# MFPKEY\_WMAAECMA\_MICARRAY\_DESCPTR Property

Specifies the microphone array geometry for the Voice Capture DSP.

## Constant for IPropertyBag

Available only by using [**IPropertyStore**](https://msdn.microsoft.com/e995aaa1-d4c9-475f-b1fa-b9123cd5b653).

## Data Type

VT\_BLOB

## Applies To

-   [Voice Capture DSP](voicecapturedmo.md)

## Remarks

The value of this property is a [**KSAUDIO\_MIC\_ARRAY\_GEOMETRY**](https://msdn.microsoft.com/49b8f602-8f82-4445-98f2-a63563689561) structure. This structure is defined in the header file KsMedia.h. To get the microphone array geometry, query the audio device for the KSPROPERTY\_AUDIO\_MIC\_ARRAY\_GEOMETRY property by calling the **IKsControl::KSProperty** method on the device. For more information on microphone arrays, download the white paper [How to Build and Use Microphone Arrays for Windows Vista](http://go.microsoft.com/fwlink/p/?linkid=180527).

Set this property if you are using the DSP in filter mode and microphone array processing is enabled. If you are using the DSP in source mode, the DSP automatically queries the device for the geometry information.

## Requirements



|                                     |                                                                                         |
|-------------------------------------|-----------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows Vista \[desktop apps only\]<br/>                                          |
| Minimum supported server<br/> | Windows Server 2008 \[desktop apps only\]<br/>                                    |
| Header<br/>                   | <dl> <dt>Wmcodecdsp.h</dt> </dl> |



## See also

<dl> <dt>

[Media Foundation Properties](media-foundation-properties.md)
</dt> <dt>

[Voice Capture DSP](voicecapturedmo.md)
</dt> </dl>

 

 



