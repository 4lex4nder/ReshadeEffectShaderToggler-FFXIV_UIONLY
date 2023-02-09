# ReshadeEffectShaderToggler-FFXIV_UIONLY
Applies reshade effects before UI is drawn in FFXIV. May or may not crash everything. Rushed, hacky, and messy.

# Instructions for non-Steam users
1. Quit the game
2. Click on the green "Code" button in the top right of this page then on "Download ZIP"
3. From the downloaded archive, put \*.addon into C:\Program Files (x86)\SquareEnix\FINAL FANTASY XIV - A Realm Reborn\game
4. If you're using Dalamud/XIVLauncher, put \*.ini into C:\Program Files (x86)\SquareEnix\FINAL FANTASY XIV - A Realm Reborn\game as well. Otherwise, move it to C:\Program Files (x86)\SquareEnix\FINAL FANTASY XIV - A Realm Reborn\boot
5. Start the game
6. Open ReShade overlay -> Goto tab "Add-ons" -> Enable "Copy depth buffer before clear operations" under "Generic Depth"

# Instructions for Steam users
1. Quit the game
2. Click on the green "Code" button in the top right of this page then on "Download ZIP"
3. Select the game in your Steam library and click on the cogwheel on the right side of the "PLAY" button -> Manage -> Browse local files
4. In the explorer window that opens up, place the \*.addon file from the downloaded archive in the "game" subfolder
5. If you're using Dalamud/XIVLauncher, put \*.ini into the "game" subfolder as well. Otherwise just leave it in the folder that originally opened up (i.e., the level above "game"/"boot")
6. Start game
7. Open ReShade overlay -> Goto tab "Add-ons" -> Enable "Copy depth buffer before clear operations" under "Generic Depth"

# Notes
* Use any ingame gamma display setting that is not exactly 50
* If you have "FFKeepUI" and/or "FFRestoreUI" effects enabled, disable them
* Try to avoid having multiples of the same effects hidden somewhere in nested folders in ReShade's Shader directory
* Disable Dynamic Resolution in-game
* Set game to DirectX 11 and Settings to Max, except for Anti-Aliasing and Ambient Occlusion, which can be whatever. You can further adjust after making sure everything works to verify nothing breaks on changing the settings

# Known issues
* ~~If no UI is rendered, effects will be applied onto the whole screen (including ReShade overlay)~~
* ~~Effects are not visible on screenshots if no UI is rendered (e.g. scroll lock). Might need to use Print screen or SHIFT+ALT+S for now~~: Enable "Clear alpha channel" in ReShade settings