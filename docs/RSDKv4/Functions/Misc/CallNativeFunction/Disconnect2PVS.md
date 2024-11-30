# Disconnect2PVS

## Description

Ends the currently active 2P VS session.

## Parameters

`entityID`

: sends the entity in the `entityID` slot to the other player in the 2PVS session.

`unused`

: unused paramater

## Return Value

None.

## Syntax

```
CallNativeFunction2(Disconnect2PVS, int entityID, int unused)
```

## Example

```
CallNativeFunction2(Disconnect2PVS)
```