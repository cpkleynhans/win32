---
title: SetInt32Property method of the Win32_RDMSDeploymentSettings class
description: Updates an integer property for the deployment settings of a virtual desktop collection.
ms.assetid: c5e6dbd5-7db7-4409-bf53-c2680e4a5319
ms.tgt_platform: multiple
keywords:
- SetInt32Property method Remote Desktop Services
- SetInt32Property method Remote Desktop Services , Win32_RDMSDeploymentSettings class
- Win32_RDMSDeploymentSettings class Remote Desktop Services , SetInt32Property method
topic_type:
- apiref
api_name:
- Win32_RDMSDeploymentSettings.SetInt32Property
api_location:
- RDMS.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
---

# SetInt32Property method of the Win32\_RDMSDeploymentSettings class

Updates an integer property for the deployment settings of a virtual desktop collection.

## Syntax


```mof
uint32 SetInt32Property(
  [in] string Key,
  [in] sint32 Value
);
```



## Parameters

<dl> <dt>

*Key* \[in\]
</dt> <dd>

The alias to the virtual desktop collection.

</dd> <dt>

*Value* \[in\]
</dt> <dd>

The new property value.

</dd> </dl>

## Requirements



| Requirement | Value |
|-------------------------------------|---------------------------------------------------------------------------------------------|
| Minimum supported client<br/> | None supported<br/>                                                                   |
| Minimum supported server<br/> | Windows Server 2012<br/>                                                              |
| Namespace<br/>                | Root\\CIMv2\\rdms<br/>                                                                |
| MOF<br/>                      | <dl> <dt>RDManagement.mof</dt> </dl> |
| DLL<br/>                      | <dl> <dt>RDMS.dll</dt> </dl>         |



## See also

<dl> <dt>

[**Win32\_RDMSDeploymentSettings**](win32-rdmsdeploymentsettings.md)
</dt> </dl>

 

 





