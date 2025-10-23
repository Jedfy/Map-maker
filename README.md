## Map-maker
This is the public repository for an app to make maps for the team game mod. Working Exe file is downloadable. (this is vibe coded and ugly code, but it works)

##Wiki

#Add System
Click Add System, then left-click on the canvas to place a star.
A yellow dot appears; label shows the primary attribute once set.

#Build Hyperlane
Click Build Hyperlane → left-click first system, then second.
Enter type (1–6). Color key: 1 white, 2 yellow, 3 red, 4 green, 5 pink, 6 blue.

#Modify System Coordinates
Click Modify System Coordinates → left-click a system → enter new X, Y.

#Add / Delete Attributes
Add Attributs → click a system → choose an index from systems_initializers.xlsx.
The first attribute in the set is the displayed label and the one used on export.

#Delete Attributs → click a system to clear its attributes.

#Back / Cancel Back
Back: removes the last hyperlane; if none, removes the last system.
Cancel Back: restores the last removed item.

#Symetry: mirror selected systems and their lines.
Options: horizontal (mirror Y), vertical (mirror X), center (180°).
Creates only lines among the newly mirrored systems.

#Copy-Paste: duplicates selected systems/lines by an offset (dx, dy) you enter.

#Delete: removes selected systems and attached lines; IDs are reindexed.

#Save / Load
Save Data: writes a project .txt with {"points": …, "lines": …}.
Load Data: reloads a saved project and redraws the scene.

#Export Galaxy
Writes a complete static_galaxy_scenario file.
Prompts:
filename, 2) team format (1v1, 2v2, …, 2v6), 3) team positions (left_vs_right or top_vs_bottom).
It will export the galaxy for team game mod formet.
