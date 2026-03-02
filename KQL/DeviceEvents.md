###Shows ActionType values for DeviceEvents, counts them per value, and sorts them in descending order. Helpful for table exploration.
DeviceEvents
| summarize Count = count()by ActionType
| sort by Count desc
