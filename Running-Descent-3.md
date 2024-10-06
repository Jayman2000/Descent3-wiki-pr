![d3 (1)](https://github.com/DescentDevelopers/Descent3/assets/47716344/8fa6bf0e-0ec0-4130-8fad-fa20bbd93a31)

# Table of Contents
1. [System Requirements](https://github.com/DescentDevelopers/Descent3/wiki/Running-Descent-3#system-requirements)
2. [Command-Line Options](https://github.com/DescentDevelopers/Descent3/wiki/Running-Descent-3#command-line-options)
3. [Debug Commands](https://github.com/DescentDevelopers/Descent3/wiki/Running-Descent-3#debug-commands)
4. [Multiplayer Compatibility](https://github.com/DescentDevelopers/Descent3/wiki/Running-Descent-3#multiplayer-compatibility)

# System Requirements
Disclaimer: These are the legacy requirements, so we use them as our base. As we made modernization changes, requirements to run Descent 3 may change.

Minimum:

- A 200MHz Pentium processor
- 32MB RAM
- 3D accelerator video card with 4 MB of texture RAM
- 210 MB hard disk space
- DirectX 6 certified sound card
- If you have Windows 95 or Windows 98, DirectX 6.1 software
- If you have Windows NT 4.0, Service Pack 3 or greater

Recommended:  

- A Pentium II 300MHz processor
- 64MB RAM
- 500 MB hard disk space

# Debug Commands
When using the debug build of Descent 3, the following keyboard debug combinations are available. These debug keys require you to press DEL in addition to the key combination below.

| Key Combination          | Action                                         |
|--------------------------|------------------------------------------------|
| Shift + Backspace        | Debug break                                    |
| Shift + Left Bracket     | Multiplayer: Send request to play taunt 0      |
| Shift + Right Bracket    | Multiplayer: Send request to play taunt 1      |
| DEL + A				   | Toggle AI (on/off)                             |
| DEL + B            	   | Cycle through game sphere rendering modes      |
| DEL + C            	   | Switch cockpit display modes                   |
| DEL + D            	   | Cycle through dynamic lighting modes           |
| DEL + E            	   | Cycle through exit sequence cameras            |
| DEL + F            | Switch rendering effects on/off                 |
| DEL + G            | Print current OpenGL information                |
| DEL + H            | Toggle HUD visibility                          |
| DEL + I            | Drop current primary weapon                    |
| DEL + J            | Teleport player to crosshair location          |
| DEL + K            | Clear all bots from current level               |
| DEL + L            | Load level by name                              |
| DEL + M            | Toggle morphing cheat                           |
| DEL + N            | Move player to next segment                    |
| DEL + O            | Cycle through object rendering modes            |
| DEL + P            | Move player to previous segment                |
| DEL + Q            | Add laser to object under crosshair            |
| DEL + R            | Restart level                                   |
| DEL + S            | Save game                                       |
| DEL + T            | Move time forward by 10 seconds                |
| DEL + U            | Move time backward by 10 seconds               |
| DEL + V            | Cycle through cockpit views                    |
| DEL + W            | Cycle through weapons                          |
| DEL + X            | Show/Hide extras menu                          |
| DEL + Y            | Cycle through mine rendering modes              |
| DEL + Z            | Cycle through all key-sets                    |
| DEL + 0-9          | Cheats (see list below)                       |
| DEL + Keypad 0-9   | Select primary weapon number                 |
| DEL + PgUp/PgDn    | Increase/Decrease time acceleration           |
| DEL + Shift + R    | Reload all level textures                      |
| DEL + Shift + T    | Reset time acceleration                        |
| DEL + Shift + W    | Set current primary weapon energy             |
| DEL + Alt + B      | Show briefings for current level              |
| DEL + Alt + L      | Toggle lightning cheat                        |
| DEL + Alt + R      | Show author info for current level            |
| DEL + Alt + S      | Show ending sequence for current level        |
| DEL + Alt + U      | Show credits for current level                |
| DEL + Alt + Shift + S | Play sound with current sound index        |
| DEL + Alt + Shift + V | Play video with current video index        |
| DEL + Shift + Left Arrow | Decrease fog density                        |
| DEL + Shift + Right Arrow | Increase fog density                       |
| DEL + Shift + Up Arrow | Increase haze level                          |
| DEL + Shift + Down Arrow | Decrease haze level                        |
| DEL + Shift + NUMPAD_Multiply | Increase flight level                        |
| DEL + Shift + NUMPAD_Divide | Decrease flight level                         |
| DEL + Shift + NUMPAD_Add | Set flight level to 0                         |
| DEL + Shift + NUMPAD_Subtract | Set flight level to 1                       |
| DEL + Shift + NUMPAD_Enter | Set flight level to 2                         |
| DEL + Shift + NUMPAD_Decimal | Set flight level to 3                       |
| DEL + Alt + Shift + Left Arrow | Move left stereo channel forward        |
| DEL + Alt + Shift + Right Arrow | Move right stereo channel forward      |
| DEL + Alt + Shift + Up Arrow | Increase stereo channel level               |
| DEL + Alt + Shift + Down Arrow | Decrease stereo channel level             |
| DEL + Alt + Shift + NUMPAD_Multiply | Reset stereo channels to normal        |
| DEL + Alt + Shift + NUMPAD_Divide | Enable stereo inversion                    |
| DEL + Alt + Shift + NUMPAD_Add | Disable stereo inversion                    |
| DEL + Alt + Shift + NUMPAD_Subtract | Toggle stereo separation               |
| DEL + Alt + Shift + NUMPAD_Enter | Toggle stereo separation                   |
| DEL + Alt + Shift + NUMPAD_Decimal | Cycle through stereo separation modes   |
| DEL + Alt + Shift + Spacebar | Toggle 3d head movement                      |
| DEL + Alt + Shift + Backspace | Toggle low framerate warning              |
| DEL + Alt + Shift + A | View (local) actor status                     |
| DEL + Alt + Shift + B | View (local) behavior status                  |
| DEL + Alt + Shift + C | View control center status                    |
| DEL + Alt + Shift + D | View dynamics status                          |
| DEL + Alt + Shift + E | View effects status                           |
| DEL + Alt + Shift + F | View physics status                           |
| DEL + Alt + Shift + G | View general status                           |
| DEL + Alt + Shift + H | View hard-coded status                        |
| DEL + Alt + Shift + I | View (local) information status               |
| DEL + Alt + Shift + J | View join-closing status                      |
| DEL + Alt + Shift + K | View (local) control status                   |
| DEL + Alt + Shift + L | View lighting status                          |
| DEL + Alt + Shift + M | View missions status                          |
| DEL + Alt + Shift + N | View network status                           |
| DEL + Alt + Shift + O | View objects status                           |
| DEL + Alt + Shift + P | View pathfinding status                       |
| DEL + Alt + Shift + Q | View physics status                           |
| DEL + Alt + Shift + R | View render status                            |
| DEL + Alt + Shift + S | View sound status                             |
| DEL + Alt + Shift + T | View texture status                           |
| DEL + Alt + Shift + U | View (local) update status                    |
| DEL + Alt + Shift + V | View vision status                            |
| DEL + Alt + Shift + W | View weapon status                            |
| DEL + Alt + Shift + X | View text status                              |
| DEL + Alt + Shift + Y | View play status                              |
| DEL + Alt + Shift + Z | View animation status                         |
| DEL + Alt + Shift + Spacebar | View spatial partition status          |
| DEL + Alt + Shift + 1 | View join-closing status                      |
| DEL + Alt + Shift + 2 | View leave-closing status                     |
| DEL + Alt + Shift + 3 | View multicast status                         |
| DEL + Alt + Shift + 4 | View network status                           |
| DEL + Alt + Shift + 5 | View objects status                           |
| DEL + Alt + Shift + 6 | View packet status                            |
| DEL + Alt + Shift + 7 | View time control status                      |
| DEL + Alt + Shift + 8 | View transport status                         |
| DEL + Alt + Shift + 9 | View update status                            |
| DEL + Alt + Shift + 0 | View version status                           |
| DEL + Alt + Shift + - | View multi-team status                        |
| DEL + Alt + Shift + = | View sync status                              |

# Multiplayer Compatibility
To play Descent 3 v1.5 multiplayer, you will need a 1.4-patched `dfmc.dll` file: the version from the CD will not work. You can connect to the following 1.5 servers:

`96.9.208.115:2092` - Hosted by DescentMax7930, v1.5 Stable  
`64.44.131.41:2092` - Hosted by DescentMax7930, [Piccu Engine](https://github.com/InsanityBringer/PiccuEngine) (by InsanityBringer)

Bear in mind that v1.5 Stable is not perfect and multiplayer is largely untested as of yet. Please have fun while testing and report issues as encountered.