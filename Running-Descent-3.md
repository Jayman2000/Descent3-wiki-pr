![d3 (1)](https://github.com/DescentDevelopers/Descent3/assets/47716344/8fa6bf0e-0ec0-4130-8fad-fa20bbd93a31)

# Table of Contents
1. [System Requirements](https://github.com/DescentDevelopers/Descent3/wiki/Running-Descent-3#system-requirements)
2. [Command-Line Options](https://github.com/DescentDevelopers/Descent3/wiki/Running-Descent-3#command-line-options)
3. [Debug Commands](https://github.com/DescentDevelopers/Descent3/wiki/Running-Descent-3#debug-commands)
4. [Multiplayer Compatibility](https://github.com/DescentDevelopers/Descent3/wiki/Running-Descent-3#multiplayer-compatibility)

## System Requirements
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

## Command-Line Options
The following command-line options are available in Descent 3. You can set command-line options on the Misc. tab of the Setup section of the Descent 3 launcher or by creating a shortcut to `main.exe`. Case is not significant in command-line options.

| **Display Options**       | **Description**                                                                                       |
|---------------------------|-------------------------------------------------------------------------------------------------------|
| `-aspect <value>`         | Specifies the screen aspect ratio for non-standard displays, such as wide-screen TVs.                |
| `-height <height>`        | Sets the screen resolution to the specified height, if possible.                                       |
| `-himem`                  | Forces normal operations even when low memory conditions are detected.                                  |
| `-lowmem`                 | Uses scaled-down textures and lower quality (8-bit) sounds to conserve memory.                          |
| `-NoRenderWindows`        | Causes all windows to be fully transparent. Use this option if your card does not correctly render partially-transparent windows. |
| `-superlowmem`            | Uses the `-lowmem` settings and further scales down textures to conserve memory.                        |
| `-vsync`                  | Turns on Vertical Sync. The flag will be enabled in the registry so it will be on when the game is run again. |
| `-width <width>`          | Sets the screen resolution to the specified width, if possible.                                        |
| `-windowed`               | Runs the game in a window.                                                                            |
| `-z32bit`                 | Enables the 32-bit z-buffer on cards that support it, such as the Matrox G400.                         |

| **Audio Options**         | **Description**                                                                                       |
|---------------------------|-------------------------------------------------------------------------------------------------------|
| `-nomusic`                | Disables music.                                                                                       |
| `-nosound`                | Disables all sound, including music.                                                                  |

| **Controls Options**      | **Description**                                                                                       |
|---------------------------|-------------------------------------------------------------------------------------------------------|
| `-alternatejoy -directinput` | Causes DirectInput to be used for the joystick or other game controller, instead of standard Windows API. |
| `-chpro`                  | Enables a CH Flightstick Pro or compatible joystick.                                                  |
| `-deadzone# <k>`          | Specifies the size of the deadzone for a joystick.                                                     |
| `-mlooksens <scale>`      | Determines how much the player moves when the mouse is moved.                                          |
| `-mouseman`               | Enables special handling for the Logitech MouseMan.                                                     |
| `-mousesens <scale>`      | Adjusts the sensitivity of the mouse when not using mouselook mode.                                     |

| **Performance Options**   | **Description**                                                                                       |
|---------------------------|-------------------------------------------------------------------------------------------------------|
| `-bumped`                 | Enables hardware bump-mapping on cards that support it, such as the Matrox G400.                      |
| `-fastdemo`               | Causes a demo to play back at the highest speed your computer is capable of.                           |
| `-forcelightmaps`         | Forces the use of lightmaps, even the Default Detail Level is set to Low in the launcher setup.       |
| `-framecap <fps>`         | Limits the framerate to the number of frames per second specified.                                      |
| `-highvidmem`             | Causes 2 MB Voodoo 1 cards to behave as if they had more memory.                                        |
| `-nocompress`             | Turns off S3TC texture compression for cards that support it.                                           |
| `-nolightmaps`            | Disables lightmaps. This will improve performance on low-end video cards.                               |
| `-nomotionblur`           | Disables motion blur on robots (Pentium III only).                                                      |
| `-nomultitexture`         | Disables single-pass multitexturing. This option could fix problems due to buggy drivers on future video cards. |
| `-nooutdoorfog`           | Disables fog on the terrain under Direct3D. This may improve performance on some cards.                |
| `-nopentium3`             | Disables detection of the Pentium III processor.                                                        |
| `-nosatomega`             | Disables alpha saturation on the omega cannon effect.                                                   |
| `-subpixelcorrect`        | Adjusts for subpixel correction under Direct3D for cards that do not support it.                        |
| `-nosparkles`             | Disables powerup sparkles (Pentium III only).                                                           |

| **Multiplayer and Network Options** | **Description**                                                                                   |
|-------------------------------------|---------------------------------------------------------------------------------------------------|
| `-audiotauntdelay <time>`          | Sets the time in seconds the a user must wait after sending an audio taunt before he or she is able to send another. This option is only active when starting a server. |
| `-autoexec <file>`                 | Specifies the full path and file name of the multiplayer config file to be loaded and executed when a multiplayer game is initialized. |
| `-dedicated <config file>`         | Starts a dedicated server.                                                                        |
| `-gamespyport <port>`              | Specifies a port for to listen for GameSpy requests. The default is 20142.                         |
| `-gspyfile <config file>`          | Specifies a GameSpy configuration file to use (default is gamespy.cfg).                             |
| `-httpproxy <addr>` or `-httpproxy <addr:port>` | Specifies an HTTP proxy server. Descent 3 uses HTTP to auto-download a mission; use this option if your ISP requires a proxy server for HTTP connections. If the first form is used, the port value defaults to 80. |
| `-nooutragelogo`                   | Disables the Outrage logo that is normally displayed for five seconds at the start of a multiplayer game. |
| `-nomultibmp`                      | Disables sending or receiving in-game custom bitmaps for ships.                                      |
| `-nonetwork`                       | Disables all network multiplayer functionality.                                                      |
| `-playermessages`                  | Disables all weapon-related HUD messages in multiplayer games.                                        |
| `-pxoport <port>`                  | Specifies the port that PXO will tell clients to use when contacting a server. The default is 2092. |
| `-useip <IP>`                      | Binds Descent 3 to this IP address. Use this option to tell D3 which IP address to use if your computer has multiple IP addresses. |
| `-useport <port>`                  | Specifies the port that TCP/IP and IPX will use. The default is 2092.                                |
| `-usesmoothing`                    | Enables code to smooth the interpolation for fast-moving objects. This will fix "skipping" problems with fast weapons, such as the Phoenix. This option applies to clients only; using it on the server has no effect. |

| **Other Options**         | **Description**                                                                                       |
|---------------------------|-------------------------------------------------------------------------------------------------------|
| `-launched`               | Skips the launcher (only on `main.exe`).                                                              |
| `-makemovie`              | Causes the demo system to save a screenshot of every frame during playback.                            |
| `-mission <name>`         | Loads the specified mission file at startup.                                                           |
| `-nocrashbox`             | Disables the error dialog displayed if Descent3 crashes.                                                |
| `-pilot <name>`           | Specifies the pilot to use, skipping the pilot selection dialog when the game starts.                  |
| `-setdir <path>`          | Specifies the working directory for Descent 3.                                                         |
| `-timetest <file>`        | Causes Descent 3 to play back the specified demo file upon startup.                                     |
| `-useexedir`              | Tells Descent 3 to use the directory in which the executable is located as the working directory.      |


## Debug Commands
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

## Multiplayer Compatibility
To play Descent 3 v1.5 multiplayer, you will need a 1.4-patched `dfmc.dll` file: the version from the CD will not work. You can connect to the following 1.5 servers:

`96.9.208.115:2092` - Hosted by DescentMax7930, v1.5 Stable  
`64.44.131.41:2092` - Hosted by DescentMax7930, v1.5 Piccu fork (by InsanityBringer)

Bear in mind that v1.5 Stable is not perfect and multiplayer is largely untested as of yet. Please have fun while testing and report issues as encountered.