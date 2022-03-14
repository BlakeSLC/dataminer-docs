---
uid: GetMaskedAlarmsForServiceCached
---

# GetMaskedAlarmsForServiceCached

Use this method to retrieve only masked service alarms added or changed since a particular point in time.

> [!NOTE]
> Using this method, you can e.g. request masked service alarms in batches in order to minimize loading time.

## Input

| Item | Format | Description |
|--|--|--|
| Connection | String | The connection ID. See [ConnectApp](xref:ConnectApp). |
| DmaID | Integer | The DMA ID. |
| ServiceID | Integer | The service ID. |
| Index | Integer | The point from which to start returning alarms. |
| Count | Integer | The number of alarms to be returned. |
| OrderBy | String | The Alarm Console column(s) by which to order the alarms (separated by semicolons). |
| CacheDateUTC | Long integer | If you enter a timestamp in UTC format (milliseconds since midnight January 1, 1970 GMT), then the method will return only masked service alarms that were added or changed since that particular point in time. If you enter -1, there will be no date check. |

## Output

| Item | Format | Description |
|--|--|--|
| GetMaskedAlarmsFor­ServiceCachedResult | [DMACache](xref:DMACache) | The masked service alarms added or changed since the specified point in time. |

> [!NOTE]
> In this case, the [DMACache](xref:DMACache) object will contain an array of [DMAAlarm](xref:DMAAlarm) objects.