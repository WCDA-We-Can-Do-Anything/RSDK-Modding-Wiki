# RSDKv2 Functions

## Audio
| Function                                          | Description                                                                                            |
| ------------------------------------------------- | ------------------------------------------------------------------------------------------------------ |
| [**SetMusicTrack**](Audio/SetMusicTrack.md)       | Loads a music file in the given track slot.                                                            |
| [**PlayMusic**](Audio/PlayMusic.md)               | Plays the music currently loaded in the given track slot.                                              |
| [**StopMusic**](Audio/StopMusic.md)               | Stops playing the currently playing music track, if one is playing.                                    |
| [**PlaySfx**](Audio/PlaySfx.md)                   | Plays the sound effect in the given slot in the GameConfig or StageConfig, looping it if set to do so. |
| [**StopSfx**](Audio/StopSfx.md)                   | Stops all instances of the given sound effect playing.                                                 |
| [**SetSfxAttributes**](Audio/SetSfxAttributes.md) | Sets the loop count and panning of the given sound effect to the given values.                         |

## Drawing
| Function                                                    | Description                                                                                                                                |
| ----------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------ |
| [**DrawTintRect**](Drawing/DrawTintRect.md)                 | Draws a tinted rectangle to `ixpos` and `iypos` in screen-space.                                                                           |
| [**LoadPalette**](Drawing/LoadPalette.md)                   | Loads a palette into `palBank` starting from `startPalIndex`, with an offset of `startIndex` and reading all colors through to `endIndex`. |
| [**RotatePalette**](Drawing/RotatePalette.md)               | Rotates all colors in `palBank` from `startIndex` to `endIndex`, moving left or right depending on `rotRight`.                             |
| [**SetFade**](Drawing/SetFade.md)                           | no clue tbh                                                                                                                                |
| [**ClearScreen**](Drawing/ClearScreen.md)                   | Clears all pixels on screen with colour `clearIndex` from the active palette.                                                              |

## Graphics
| Function                                                   | Description                                                                                                                          |
| ---------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------ |
| [**LoadSpriteSheet**](Graphics/LoadSpriteSheet.md)         | Loads a spritesheet and assigns the ID to `object.spritesheet`.                                                                      |
| [**RemoveSpriteSheet**](Graphics/RemoveSpriteSheet.md)     | Removes the given spritesheet from memory, if it is already loaded.                                                                  |
| [**DrawSprite**](Graphics/DrawSprite.md)                   | Draws `frame` at the object's X and Y position.                                                                                      |
| [**DrawSpriteXY**](Graphics/DrawSpriteXY.md)               | Draws `frame` at a specified X and Y position.                                                                                       |
| [**DrawSpriteScreenXY**](Graphics/DrawSpriteScreenXY.md)   | Draws `frame` at a specified X and Y position in screen-space.                                                                       |
| [**SpriteFrame**](Graphics/SpriteFrame.md)                 | Adds a SpriteFrame with the specified values.                                                                                        |
| [**DrawSpriteFX**](Graphics/DrawSpriteFX.md)               | Draws `frame` at a specified X and Y position with visual effects.                                                                   |
| [**DrawSpriteScreenFX**](Graphics/DrawSpriteScreenFX.md)   | Draws `frame` at a specified X and Y position in screen-space with visual effects.                                                   |

## Math
| Function                                   | Description                                                                                           |
| ------------------------------------------ | ----------------------------------------------------------------------------------------------------- |
| [**Rand**](Math/Rand.md)                   | Gets a random value from 0 to `max` (not inclusive) and stores it in `store`.                         |
| [**Sin**](Math/Sin.md)                     | Gets the value from the `sin512` lookup table based on `angle` and sets it in `store`.                |
| [**Cos**](Math/Cos.md)                     | Gets the value from the `cos512` lookup table based on `angle` and sets it in `store`.                |
| [**Sin256**](Math/Sin256.md)               | Gets the value from the `sin256` lookup table based on `angle` and sets it in `store`.                |
| [**Cos256**](Math/Cos256.md)               | Gets the value from the `cos256` lookup table based on `angle` and sets it in `store`.                |
| [**ATan2**](Math/ATan2.md)                 | Performs an arctan operation using `x` and `y`, storing the result in `store`.                        |
| [**Interpolate**](Math/Interpolate.md)     | Linearly interpolates `x` and `y` by `percent` and stores the result in `store`.                      |
| [**InterpolateXY**](Math/InterpolateXY.md) | Linearly interpolates two points at once and stores the result in `storeX` and `storeY` respectively. |
| [**Not**](Math/Not.md)                     | Performs a NOT operation on `value`.                                                                  |

## Object
| Function                                                   | Description                                                                                                                 |
| ---------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------- |
| [**CreateTempObject**](Object/CreateTempObject.md)         | Creates a temporary object specified by `type`, `propertyValue`, `xpos` and `ypos` near the end of the object list.         |
| [**ProcessObjectControl**](Object/ProcessObjectControl.md) | Handles object input variables.                                                                                             |
| [**ObjectTileCollision**](Object/ObjectTileCollision.md)   | Tries to collide with the foreground layer based on the position of `object.ixpos` + `xOffset`, `object.iypos` + `yOffset`. |
| [**ObjectTileGrip**](Object/ObjectTileGrip.md)             | Tries to collide with the foreground layer based on the position of `object.ixpos` + `xOffset`, `object.iypos` + `yOffset`. |

## Stages
| Function                                                         | Description                                                                               |
| ---------------------------------------------------------------- | ----------------------------------------------------------------------------------------- |
| [**LoadStage**](Stages/LoadStage.md)                             | Loads a stage based on `stage.activeList` and `stage.listPos`.                            |

## Miscellaneous
| Function                                   | Description                                                                                              |
| ------------------------------------------ | -------------------------------------------------------------------------------------------------------- |
| [**SetupMenu**](Misc/SetupMenu.md)         | Sets up `menu` with `rowCount` rows, `selectionCount` active selections and aligning set to `alignment`. |
| [**AddMenuEntry**](Misc/AddMenuEntry.md)   | Adds an entry to `menu` with the contents of `text`.                                                     |
| [**EditMenuEntry**](Misc/EditMenuEntry.md) | Edits an entry of `menu` with the contents of `text` in `rowID`.                                         |
| [**DrawMenu**](Misc/DrawMenu.md)           | Draws `menu` at `xpos` and `ypos` relative to the screen.                                                |
| [**LoadTextFile**](Misc/LoadTextFile.md)   | Loads `menu` based on the text file loaded from `filePath`.                                              |
