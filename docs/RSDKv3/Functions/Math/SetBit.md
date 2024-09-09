# SetBit

## Description
Sets index `BitPos` of `Value` to `Bit` and updates `Value` accordingly.

## Parameters
- `Value`
The variable to update.
- `BitPos`
The position of the bit to set, indices 0-7 are valid.
- `Bit`
Updated boolean value.

## Return Value
None.

## Syntax
```
SetBit(var Value, int BitPos, bool Bit)
```

## Examples
```
SetBit(Object.Value7, 3, 1)
```