# Low Game Events

https://docs.fivem.net/docs/scripting-reference/events/list/gameEventTriggered/

## CEventShockingGunshotFired

This event get trigger when a NPC hear or see a gunshot

| Args | Type | Description |
| ------ | ------ | ------ |
| a | table | All the NPC involved or yourself
| b | number | Ped, generally is  PlayerPedId()
| c | table | Coordinates of the event

```lua
AddEventHandler("CEventShockingGunshotFired",function(a,b,c) 
 local Player = a[1] -- PlayerPedId()
 local PlayerAgain = b -- PlayerPedId()
 local TableCoords = c[1] -- table with coords
 local Coords = vector3(TableCoords[1],TableCoords[2],TableCoords[3]) 
end)
```
## CEventShockingMadDriverExtreme and CEventShockingMadDriver

This event get trigger when you pass an NPC at hight speed or when you drive like crazy thowards a ped

| Args | Type | Description |
| ------ | ------ | ------ |
| a | table | All the NPC involved or yourself
| b | number | Ped, generally is  PlayerPedId()
| c | table | Coordinates of the event


```lua
AddEventHandler("CEventShockingMadDriverExtreme",function(a,b,c) 
    local Player = a[1] 
    local PlayerAgain = b -- PlayerPedId()
    local TableCoords = c[1] -- table with coords
    local Coords = vector3(TableCoords[1],TableCoords[2],TableCoords[3]) 
end)
```
