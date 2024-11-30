# SetWindowVSync

## Description
Allows `ApplyWindowChanges` to turn on or off VSync.

## Parameters
`vSync`

:   The value that you want to change VSync to.

`unused`

:   Unused parameter.

## Return Value
None.

## Syntax
```
CallNativeFunction2(SetWindowVSync, bool vSync, int unused)
```

## Example
```
CallNativeFunction2(SetWindowVSync, true, 0)
```