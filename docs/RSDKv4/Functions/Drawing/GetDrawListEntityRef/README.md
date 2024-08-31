# GetDrawListEntityRef

## Description
Gets `objectPos` in the drawList layer and stores it in `store`

## Parameters
- `layer`
layer of the drawList to add the reference, indices 0-7 are valid, additionally 8 is available in V5U.
- `objectPos`
the position of the object to add
- `store`
the variable where `objectPos` will be stored

## Return Value
None.

## Syntax
```GetDrawListEntityRef(var Store, int Layer, int objectPos)```

## Examples
- ```GetDrawListEntityRef(object.value0, 4, object.entityPos)```