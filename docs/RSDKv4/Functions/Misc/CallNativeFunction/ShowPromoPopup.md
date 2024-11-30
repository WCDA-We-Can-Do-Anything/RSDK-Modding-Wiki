# ShowPromoPopup

## Description

Attempts to display a promotional popup. 

**NOTE**: This function does nothing on the decompilation.

## Parameters

`id`

:   The id of the popup.

`promoName`

:   Name of the promotional popup.

## Return Value

None.

## Syntax

```
CallNativeFunction2(ShowPromoPopup, int id, string promoName)
```

## Example

```
CallNativeFunction2(ShowPromoPopup, 0, "GameOverPromo")
```