# ReshadeEffectShaderToggler-FFXIV_UIONLY
Applies reshade effects before UI is drawn in FFXIV. May or may not crash everything. Rushed, hacky, and messy.

# Instructions
1. Put \*.addon and  \*.ini files into C:\Program Files (x86)\SquareEnix\FINAL FANTASY XIV - A Realm Reborn\game
2. Restart game
3. Open ReShade overlay -> Goto tab "Add-ons" -> Enable "Copy depth buffer before clear operations" under "Generic Depth"

# Notes
* Try to avoid having multiples of the same effects hidden somewhere in nested folders in ReShade's Shader directory
* Disable Dynamic Resolution in-game
* Set game to DirectX 11 and Settings to Max, except for Anti-Aliasing and Ambient Occlusion, which can be whatever. You can further adjust after making sure everything works to verify nothing breaks on changing the settings

# Known issues
* If no UI is rendered, effects will be applied onto the whole screen (including ReShade overlay).