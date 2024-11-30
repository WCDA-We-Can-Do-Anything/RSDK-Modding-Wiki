# Connect2PVS

## Description
Initializes a 2P VS session.

## Parameters
`gameLength`
Sets the number of rounds in the 2PVS session.
`itemMode`
Sets the types of items you can use in the 2PVS session.

# Game Lengths
| ID |  Game Lengths            |
| -- | ------------------------ |
| 0  | No Preference            |
| 1  | 1 Match                  |
| 2  | 2 Matches                |
| 3  | 3 Matches                |
| 4  | 4 Matches                |
| 5  | 5 Matches                |
| 6  | 6 Matches                |
| 7  | 7 Matches                |
| 8  | 8 Matches                |

# Item Modes
| ID |  Items Modes             |
| -- | ------------------------ |
| 0  | No Preference            |
| 1  | Random                   | 
| 2  | Teleport Only            |
| 3  | Fixed                    |

## Return Value
None.

## Syntax
```
CallNativeFunction2(Connect2PVS, int gameLength, int itemMode)
```

## Example
```
CallNativeFunction2(Connect2PVS, 0, 1)
```
