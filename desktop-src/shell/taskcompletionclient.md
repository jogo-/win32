---
Description: Enables task completion.
ms.assetid: 323343D6-FC4A-4A5F-B065-DD72B6077F99
title: TaskCompletionClient interface
ms.technology: desktop
ms.prod: windows
ms.author: windowssdkdev
ms.topic: interface
ms.date: 05/31/2018
---

# TaskCompletionClient interface

Enables task completion.

## Members

The **TaskCompletionClient** interface inherits from the [**IUnknown**](https://msdn.microsoft.com/windows/desktop/33f1d79a-33fc-4ce5-a372-e08bda378332) interface. **TaskCompletionClient** also has these types of members:

-   [Methods](#methods)

### Methods

The **TaskCompletionClient** interface has these methods.



| Method                                                                    | Description                            |
|:--------------------------------------------------------------------------|:---------------------------------------|
| [**ApplyTaskCompletion**](taskcompletionclient-applytaskcompletion.md)   | Begins the task completion.<br/> |
| [**RevokeTaskCompletion**](taskcompletionclient-revoketaskcompletion.md) | Ends the task completion.<br/>   |



 

## Remarks

The GUID for this interface is "E97D552D-9AE9-46AA-9151-D2DA4BBB5E96".

This API is deprecated and may not be available in future versions of Windows. Apps should use the APIs in the [**Windows.ApplicationModel.ExtendedExecution**](https://www.bing.com/search?q=**Windows.ApplicationModel.ExtendedExecution**) namespace instead.

## Requirements



|                                     |                                                                                                |
|-------------------------------------|------------------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows 10 \[desktop apps only\]<br/>                                                    |
| Minimum supported server<br/> | Windows Server 2016 \[desktop apps only\]<br/>                                           |
| DLL<br/>                      | <dl> <dt>ExecModelClient.dll</dt> </dl> |



 

 



