---
Description: Releases the handle to a cryptographic service provider (CSP) and optionally deletes the temporary container created by the GetCryptProvFromCert function.
ms.assetid: 4462eef2-7056-4e48-aa96-c46f29b701d6
title: FreeCryptProvFromCert function
ms.technology: desktop
ms.prod: windows
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# FreeCryptProvFromCert function

> \[!Important\]  
> This API is deprecated. Microsoft may remove this API in future releases.

 

The **FreeCryptProvFromCert** function releases the handle to a [*cryptographic service provider*](security.c_gly#-security-cryptographic-service-provider-gly) (CSP) and optionally deletes the temporary container created by the [**GetCryptProvFromCert**](getcryptprovfromcert.md) function.

> [!Note]  
> This function has no associated header file or import library. To call this function, you must create a user-defined header file and use the [**LoadLibrary**](https://msdn.microsoft.com/d936b4dd-058c-48e1-834b-b47ef6d8ef65) and [**GetProcAddress**](https://msdn.microsoft.com/a0d7fc09-f888-4f46-a571-d3719a627597) functions to dynamically link to Mssign32.dll.

 

## Syntax


```C++
void WINAPI FreeCryptProvFromCert(
  _In_     BOOL       fAcquired,
  _In_     HCRYPTPROV hProv,
  _In_opt_ LPWSTR     pwszCapiProvider,
  _In_     DWORD      dwProviderType,
  _In_opt_ LPWSTR     pwszTmpContainer
);
```



## Parameters

<dl> <dt>

*fAcquired* \[in\]
</dt> <dd>

A value that specifies whether the provider handle was acquired from the [*certificate*](security.c_gly#-security-certificate-gly).

</dd> <dt>

*hProv* \[in\]
</dt> <dd>

A pointer to an [**HCRYPTPROV**](hcryptprov.md) structure for the CSP.

</dd> <dt>

*pwszCapiProvider* \[in, optional\]
</dt> <dd>

A pointer to a null-terminated string for the provider name.

</dd> <dt>

*dwProviderType* \[in\]
</dt> <dd>

Specifies the CSP type. This can be zero or one of the [Cryptographic Provider Types](cryptographic-provider-types.md). If this member is zero, the key container is one of the CNG key storage providers.

</dd> <dt>

*pwszTmpContainer* \[in, optional\]
</dt> <dd>

A pointer to a null-terminated string for the name of the temporary key container.

</dd> </dl>

## Return value

This function does not return a value.

## Requirements



|                                     |                                                                                         |
|-------------------------------------|-----------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows XP \[desktop apps only\]<br/>                                             |
| Minimum supported server<br/> | Windows Server 2003 \[desktop apps only\]<br/>                                    |
| DLL<br/>                      | <dl> <dt>Mssign32.dll</dt> </dl> |



 

 



