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
|E1M1| ?       |E1M1 |WILV00  |E1M2| ?        |SKY1      |D_E1M1|idk    |             |false         |          |clear     |
|E1M2| ?       |E1M2 |WILV01  |E1M3| ?        |SKY1      |D_E1M1|idk    |             |false         |          |clear     |
|E1M3| ?       |E1M3 |WILV02  |E1M4|E1M9      |SKY1      |D_E1M1|idk    |             |false         |          |clear     |
|E1M4| ?       |E1M4 |WILV03  |E1M5| ?        |SKY1      |D_E1M1|idk    |             |false         |          |clear     |
|E1M5| ?       |E1M5 |WILV04  |E1M6| ?        |SKY1      |D_E1M1|idk    |             |false         |          |clear     |
|E1M6| ?       |E1M6 |WILV05  |E1M7| ?        |SKY1      |D_E1M1|idk    |             |false         |          |clear     |
|E1M7| ?       |E1M7 |WILV06  |E1M8| ?        |SKY1      |D_E1M1|idk    |             |false         |          |clear     |
|E1M8| ?       |E1M8 |WILV07  |?   | ?        |SKY1      |D_E1M1|idk    |             |false         |          |(see below)[#e1m8-bossaction] |
|E1M9| ?       |E1M9 |WILV08  |E1M4| ?        |SKY1      |D_E1M1|idk    |             |false         |          |clear     |

#### EndGame
describe endgame/endbunny/endpic/endcast

#### Intertexts
In a separate section cause they wouldn't fit nicely in a table

#### EnterPic/ExitPic
need to describe how in doom it uses the animated maps when not set in umapinfo

#### E1M8 BossAction
The default BossAction for E1M8 is unrepresentable in UMAPINFO. The three components are specified as follows:
- `thingtype`: In ports that implement the MBF21 specification, this does not default to a specific thing type. Rather, any thing with the E1M8BOSS flag will trigger this bossaction. Otherwise, it is "BaronOfHell".
- `linespecial`: Lower all sectors tagged 666 to the highest touching floor (todo: word this better). This does not necessarily correspond to any actual line special.
- `tag`: 666

### `doom.wad`

Defaults for E1M1-E1M9 are the same as `doom1.wad`, with the following exceptions:
(im pretty sure somethings different for e1m8 but im not sure)

#### E2M8 BossAction
The default BossAction for E2M8 is unrepresentable in UMAPINFO. The three components are specified as follows:
- `thingtype`: In ports that implement the MBF21 specification, this does not default to a specific thing type. Rather, any thing with the E2M8BOSS flag will trigger this bossaction. Otherwise, it is "Cyberdemon".
- `linespecial`: exit level (todo: actually properly describe this). This does not necessarily correspond to any actual line special.
- `tag`: tag is unused

#### E3M8 BossAction
The default BossAction for E3M8 is unrepresentable in UMAPINFO. The three components are specified as follows:
- `thingtype`: In ports that implement the MBF21 specification, this does not default to a specific thing type. Rather, any thing with the E3M8BOSS flag will trigger this bossaction. Otherwise, it is "SpiderMastermind".
- `linespecial`: exit level (todo: actually properly describe this). This does not necessarily correspond to any actual line special.
- `tag`: tag is unused

#### E4M6 BossAction
The default BossAction for E4M6 is unrepresentable in UMAPINFO. The three components are specified as follows:
- `thingtype`: In ports that implement the MBF21 specification, this does not default to a specific thing type. Rather, any thing with the E4M6BOSS flag will trigger this bossaction. Otherwise, it is "Cyberdemon".
- `linespecial`: blazing door (todo: actually properly describe this). This does not necessarily correspond to any actual line special.
- `tag`: 666

#### E4M8 BossAction
The default BossAction for E4M8 is unrepresentable in UMAPINFO. The three components are specified as follows:
- `thingtype`: In ports that implement the MBF21 specification, this does not default to a specific thing type. Rather, any thing with the E4M8BOSS flag will trigger this bossaction. Otherwise, it is "SpiderMastermind".
- `linespecial`: Lower all sectors tagged 666 to the highest touching floor (todo: word this better). This does not necessarily correspond to any actual line special.
- `tag`: 666

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