# Map-maker
This is the public repository for an app to make maps for the team game mod. Working Exe file is downloadable. (this is vibe coded and ugly code, but it works) Wiki is in english, russian and chinese. Вики доступна на английском, русском и китайском языках. 维基提供英语、俄语和中文版本。Release is : https://github.com/Jedfy/Map-maker/releases/tag/v1.0.0

# Wiki

## Add System
Click Add System, then left-click on the canvas to place a star.
A yellow dot appears; label shows the primary attribute once set.

## Modify System Coordinates
Click Modify System Coordinates → left-click a system → enter new X, Y.

## Build Hyperlane
Click Build Hyperlane → left-click first system, then second.
Regular is a normal hyperlane, midgame is a hyperlane that will appear at midgame (y30) and endgame is a hyperlane that will appear at endgame (y45)

## Build Wormhole
Click Build Hyperlane → left-click first system, then second.
Regular, midgame and endgame works the same.

## Add / Delete Attributes
Add Attributs → click a system → choose an index from systems_initializers.xlsx.
The first attribute in the set is the displayed label and the one used on export.
Delete Attributs → click a system to clear its attributes.

## Back / Cancel Back
Back: Undoes the last action (ctrl-z equivalent)
Cancel Back: Undoes the last undo (ctrl-y equivalent)

## Save Data / Load Data
Save Data: writes a .txt to save your project.
Load Data: reloads a saved project and redraws the galaxy.

## Symetry
Mirrors selected systems and their hyperlanes.
Options: horizontal (mirror Y), vertical (mirror X), center (180°).

## Copy-Paste
Duplicates selected systems/lines by an offset (dx, dy) you enter.

## Circular Symetry
Mirrors selected systems and their hyperlanes, but following a revolution pattern. You can either pick :
total angle + times : total angle of revolution and the amount of times your pattern appears (including the selected systems)
step angle + copy : you pick the angle between the copies, and the amount of copies.
You can also change the center of the symetry, this is for people wanting to do multiple clusters in different parts of galaxy separatly.

## Export Galaxy
Writes a complete static_galaxy_scenario file, given your current galaxy
It will export the galaxy for team game mod format. 
Put this galaxy file in : map\setup_scenarios
The settings are :
#### team format : 
xvxvx or xvyvz here (1v1, 8v8, 2v2, 4v4v4 or 3v4v5)
#### team layout : 
this is to automatically separate spawns so that spawn 1 is at the top left corner of galaxy for example. If doesn't work properly, tweak the generated capital_system_initializer_1 into capital_system_initializer_2 or else to fix which spawn is which. But it works most of the time.
#### how many teams :
select the amount of teams on the map. if it's a 1v1 map, select the 1v1 special mode. if it's 3v3, select 2 teams. 3v3v3 3 teams, 2v4v6v7 4 teams, 2v2v2v2v2 5 teams, etc.
The mod supports up to 20 players on 10 different teams.

## Delete
Removes selected systems and hyperlanes

## About solar systems initializers
You need the systems_initializers.xlsx file in the same folder for the solar systems initializers to work properly. You can add a vanilla one in the excel file, or even make your own solar system initializers. (they are in common\solar_system_initializers). If the initializer does not exist, an error will appear on the error.log and the system will instead be a random vanilla one.
Also, there can only be 2 garantees for a player at the moment, and they can be at max 2 jumps away from the capital.


