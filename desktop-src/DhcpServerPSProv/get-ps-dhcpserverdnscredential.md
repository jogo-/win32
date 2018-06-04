---
title: Get method of the PS\_DhcpServerDnsCredential class
description: Gets the user account used by the DHCP server for registering or de-registering client records with DNS server.
audience: developer
author: REDMOND\\markl
manager: REDMOND\\markl
ms.assetid: d3e3931d-c4e6-4f0b-9390-e81ec17c3a9e
ms.prod: windows-server-dev
ms.technology:
- dhcp-server
- windows-management-instrumentation
ms.tgt_platform: multiple
keywords:
- Get method
- Get method, PS_DhcpServerDnsCredential class
- PS_DhcpServerDnsCredential class, Get method
topic_type:
- apiref
api_name:
- PS_DhcpServerDnsCredential.Get
api_location:
- DhcpServerPsProvider.dll
api_type:
- COM
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# Get method of the PS\_DhcpServerDnsCredential class

Gets the user account used by the DHCP server for registering or de-registering client records with DNS server

## Syntax


```mof
uint32 Get(
  [in]  string                  ComputerName,
  [out] DhcpServerDnsCredential cmdletOutput
);
```



## Parameters

<dl> <dt>

*ComputerName* \[in\]
</dt> <dd>

DNS name or IP address of the target computer running the DHCP server service.

</dd> <dt>

*cmdletOutput* \[out\]
</dt> <dd>

An embedded instance of a [**DhcpServerDnsCredential**](dhcpserverdnscredential.md) object.

</dd> </dl>

## Requirements



|                                     |                                                                                                     |
|-------------------------------------|-----------------------------------------------------------------------------------------------------|
| Minimum supported client<br/> | None supported<br/>                                                                           |
| Minimum supported server<br/> | Windows Server 2012 R2<br/>                                                                   |
| Namespace<br/>                | Root\\Microsoft\\Windows\\DHCP<br/>                                                           |
| MOF<br/>                      | <dl> <dt>DhcpServerPsProvider.mof</dt> </dl> |
| DLL<br/>                      | <dl> <dt>DhcpServerPsProvider.dll</dt> </dl> |



## See also

<dl> <dt>

[**PS\_DhcpServerDnsCredential**](ps-dhcpserverdnscredential.md)
</dt> </dl>

 

 




