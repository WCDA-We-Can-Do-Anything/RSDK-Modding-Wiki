# SetWindowScaleMode

## Description
Allows `ApplyWindowChanges` to set the scale mode of the game.

## Parameters
`mode`

:   The scale mode that you want to set the window to.
**NOTE**: Any value greater than 1 is invalid.

`unused`

:   Unused parameter.

## Return Value
None.

## Syntax
```
CallNativeFunction2(SetWindowScaleMode, int mode, int unused)
```

## Example
```
CallNativeFunction2(SetWindowScaleMode, 1, 0)
```