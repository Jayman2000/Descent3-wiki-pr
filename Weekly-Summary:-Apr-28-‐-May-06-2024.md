![image](https://github.com/DescentDevelopers/Descent3/assets/47716344/a772b8e6-4b2f-4606-aa3f-35208189d11b)

The Descent 3 Maintainers are not the sole contributors to this repository. Many of the below improvements and bug fixes were the result of contributors, of which we are extremely thankful.

Multiplayer servers:  
`96.9.208.115:2092` - Hosted by DescentMax7930, v1.5 Upstream  
`64.44.131.41:2092` - Hosted by DescentMax7930, Piccu Engine (by InsanityBringer)

# Weekly Summary: Apr 28 - May 06 2024

## Upstream Source
Repository Improvements:
- CI artifacts now include a copy of the GPL license.
- Added links to Steam and GOG releases of Descent 3.
- Removed some unused files.

Bug Fixes:
- Mercenary game assets like the Black Pyro and Red Guidebot were disabled for Linux and MacOS, and Windows users were unlikely to be able to use them due to missing registry entries. The game now checks for the presence of relevant `.hog` files and enables mercenary assets that way.
- The hardware cursor should no longer be active or visible in fullscreen mode.
- MacOS mouse cursor is now correctly grabbed in fullscreen mode.
- It is now possible to build `TCP~IP.d3c` in Windows.

Adjustments:
- Linux and MacOS have had some of icculus' 64bit code implemented.
- Linux and MacOS have had some of icculus' SDL2 code implemented.
- Windows users can now use esxtra mouse buttons in the configuration options.

General Updates:
- We have decided on using the `d2x` mve library. It has been traced to [Fallout 1 & 2](https://fodev.net/files/fo2/tools.html), which was reverse-engineered, and further modifications to it were made under GPL-2. We'd love some assistance with this, check out [#289](https://github.com/DescentDevelopers/Descent3/pull/289) if you're interested!
- The scope of 1.5 Stable has changed slightly. Now that we're able to import Ryan Gordon's 2020 code for Linux and Mac, we will be including that in our milestone. We have not yet decided if we will be adding those changes to Windows as well before the milestone release.
- Chatter: There is a discussion thread open regarding [game balance](https://github.com/DescentDevelopers/Descent3/discussions/274), feel free to hop in and make your mark!
- jmarshall23 aka icecoldduke has joined the maintainers! Ice has been hard at work with the internal editor, something we haven't touched. We're told it's much easier to work with than D3Edit, and hopefully we'll see more of it soon!

## Piccu Engine
[Piccu Engine](https://github.com/InsanityBringer/PiccuEngine) is a fork of the upstream repository (from April 16th) that prioritizes QoL improvements. While issues remain, the game is in a far more playable state on modern systems. 
Piccu Engine boasts a functioning window mode, has widescreen support, has enabled multiple mouse buttons, and more. It's Windows-only for now, though, and since upstream is integrating Ryan's code for other platforms, we are avoiding changes that might impede his import process.
We maintain a mutual-benefit relationship with InsanityBringer and his work, and Descentheads eager to get back into the game will find themselves feeling right at home with Piccu Engine.