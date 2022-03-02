---
uid: GetAvailableAlarmProperties
---

# GetAvailableAlarmProperties

Use this method to retrieve all properties that are available for alarm filtering. Available from DataMiner 9.5.6 onwards.

## Input

| Item       | Format | Description                                          |
|------------|--------|------------------------------------------------------|
| Connection | String | The connection ID. See [ConnectApp](xref:ConnectApp). |

## Output

| Item | Format | Description |
|--|--|--|
| GetAvailableAlarmPropertiesResult | Array of DMAProperty ([DMAProperty](xref:DMAProperty)) | An array with all properties available for alarm filtering. |