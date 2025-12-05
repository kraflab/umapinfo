# UMAPINFO Specification Rev 2.? Default Key Values

## Global defaults
### Author
Empty string: ""

## Map-specific defaults
The default values for most keys depend on both the map and the currently loaded IWAD.
are level names set in umapinfo treated differently from never setting the name?

### `doom1.wad`

|Map |Levelname|Label|LevelPic|Next|NextSecret|SkyTexture|Music |ParTime|InterBackdrop|NoIntermission|InterMusic|BossAction|
|----|---------|-----|--------|----|----------|----------|------|-------|-------------|--------------|----------|----------|
|E1M1| ?       |E1M1-|WILV00  |E1M2| ?        |SKY1      |D_E1M1|idk    |             |false         |          |clear     |

#### EndGame
describe endgame/endbunny/endpic/endcast

#### Intertexts
In a separate section cause they wouldn't fit nicely in a table

#### EnterPic/ExitPic
need to describe how in doom it uses the animated maps when not set in umapinfo

### `doom.wad`

Defaults for E1M1-E1M9 are the same as `doom1.wad`, with the following exceptions:
(im pretty sure somethings different for e1m8 but im not sure)

### `doom2.wad`

### `tnt.wad`

Defaults the same as doom2.wad except for map names (i think)
list them

### `plutonia.wad`

Defaults the same as doom2.wad except for map names (i think)
list them

### `chex.wad`

This gets mentioned in spec.md so i guess it goes here too??
even though i suspect ports vary by whether they need chex.deh for the map names and intertexts

## Episodes
describe behavior of episodes, particularly ep4 here