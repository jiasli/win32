---
title: CounterItem.GetDataAt method
description: Retrieves the specified counter value from a specific point in the graph.
ms.assetid: e8484301-4575-41ee-9c6d-a454eca0e82d
keywords:
- GetDataAt method SysMon
- GetDataAt method SysMon , CounterItem object
- CounterItem object SysMon , GetDataAt method
topic_type:
- apiref
api_name:
- CounterItem.GetDataAt
api_location:
- Sysmon.ocx
api_type:
- COM
ms.technology: desktop
ms.prod: windows
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# CounterItem.GetDataAt method

Retrieves the specified counter value from a specific point in the graph.

## Syntax


```VB
CounterItem.GetDataAt( _
  ByVal index As Long, _
  ByVal which As SysmonDataType, _
  ByRef variant As Object _
)
```



## Parameters

<dl> <dt>

*index* \[in\]
</dt> <dd>

Zero-based index of the graph point whose value you want to retrieve. Valid values range from 0 to ([**SystemMonitor.DataPointCount**](systemmonitor-datapointcount.md) - 1).

</dd> <dt>

*which* \[in\]
</dt> <dd>

Type of counter value to retrieve, for example, the average value of the counter as displayed in the graph window. For possible values, see [**SysmonDataType**](/windows/desktop/api/ISysmon/ne-isysmon-__midl___midl_itf_sysmon_0000_0000_0002).

</dd> <dt>

*variant* \[out\]
</dt> <dd>

Counter value that was retrieved.

</dd> </dl>

## Return value

This method does not return a value.

## Remarks

Use this method only if

-   [**SystemMonitor.DisplayType**](systemmonitor-displaytype.md) is set to sysmonLineGraph
-   [**SystemMonitor.DataSourceType**](systemmonitor-datasourcetype.md) is set to sysmonLogFiles or sysmonSqlLog

## Requirements



|                                     |                                                                                       |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows Vista \[desktop apps only\]<br/>                                        |
| Minimum supported server<br/> | Windows Server 2008 \[desktop apps only\]<br/>                                  |
| DLL<br/>                      | <dl> <dt>Sysmon.ocx</dt> </dl> |



## See also

<dl> <dt>

[**CounterItem**](counteritem.md)
</dt> <dt>

[**CounterItem.GetStatistics**](counteritem-getstatistics.md)
</dt> <dt>

[**CounterItem.GetValue**](counteritem-getvalue.md)
</dt> </dl>

 

 




