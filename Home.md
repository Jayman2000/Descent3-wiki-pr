# Descent 3 Open Source
Descent 3 was released as open source on 04/16/2024 and is licensed under GPL-3.0. This wiki serves as a guide to help readers understand the codebase and play the game. Our mission is to provide the best vanilla experience possible on modern hardware, starting with a "Vanilla 1.5 Stable" build and adding QoL improvements from there.

[Running Descent 3](https://github.com/DescentDevelopers/Descent3/wiki/Running-Descent-3): This page will assist in running the game and describes available CLI arguments.

## Original 1.5 Patch Notes
### Fixes

- Fixed a checksum problem introduced in 1.4 that prevented some levels from being played across platforms (for example, Windows and Linux).
- Force feedback now works under Windows 2000.
- Fixed crash starting a multiplayer game when the Black Pyro is the only allowed ship and the player is currently set to use another ship.
- Can no longer start a multiplayer game with no allowed ships.
- It's no longer possible to crash the dedicated server by typing a very long command line in telnet mode.
- Disabled cheats that are based on changing the ship weapon values in the data files.
- Mod files are now stored on http://www.descent3.com (instead of http://www.pxo.net).
- Removed support for HEAT.NET, as they're no longer in business.
- Pilot command-line arg `-pilot` or `+name` is now only checked once, not every time the main menu comes up. This fixes the problem of the game switching back to the pilot specified on the command line after the user has selected a different one.
- When the player's HUD name level is lowered by a game server, the client remembers the higher level and will revert to that level when a server allows.
- Fixed a problem with the GuideBot menu not responding to key presses after firing with the mouse.
- Saved games now properly load custom textures.
- Demos now properly load custom textures.
- Primary weapons no longer behave oddly when attempting to fire secondaries when out of secondaries.
- Fixed a rendering crash that could be caused (among other ways, probably) by a lot of chaff being detonated at once.
- Fixed some (maybe all) multiplayer ghost ship problem.
- Omega cannon energy usage is now not framerate dependent.
- Fixed crashes/slowdowns when using the omega cannon.
- Fixed a problem with the rearview camera when viewing demos of multiplayer games.
- Fixed a ghost ship problem with demos after a player respawned in a multiplayer game.
- Certain objects, such as the surface cannon in level 10, no longer interact with observers in multiplayer games.
- The stats file now contains a listing of team members in Team Anarchy, Mosterball, and Entropy.
- The results screen for team anarchy now shows the team scores.
- Don't show extra teams on team anarchy & monsterball results screens.
- Removed the Mission Status item from the HUD config menu, since there is no Mission Status HUD indicator.
- Removed the missile camera center window option, since it didn't really work (& wasn't supposed to be there in the first place). If you really want the center view, however, you can set MissileView to 1 in the registry. Note that going into the config menu will reset it, though.
- Fixed problems when video bit depth set to 32.
- Clients now can hear the server player taking omega (& other) damage.
- Fixed problems with omega cannon causing wrong amounts of damage and damage to the person firing the weapon.
- Allowed room for longer team names on results screens.
- Ping & packet loss data no longer displayed on HUD in peer-to-peer games.
- It's no longer possible to pick up a powerup in multiplayer while leaving observer mode while moving over the powerup.
- Added confirmation HUD messages when sending private messages.
- Fixed several problems unloading overlay data.
- Made `-mission` work as described; that is, it now causes the specified mission to start automatically when the game is started.
- Colored stipes now display on player ships in demo playback of multiplayer games.
- HUD gauges now work in demo playback.
- Clarified the description in readme.txt of the `-mission` command-line option. Refer to Section 7, Command-line Options, for the new description.
- Fixed a couple problems with the level auto-download system.
- In demos of multiplayer games, player ships no longer switch between models for different ships.

### New Features
- Increased by 20 the maximum number of player ships.
- Increased by 300 the maximum number of textures.
- Increased by 100 the maximum number of objects.
- Increased by 200 the maximum number of polygon models.
- Added "-nosatomega" command-line option to disable alpha effects on omega cannon. Try this if you have speed or crashing
problems with the omega under 1.5.
- Added -nocrashbox command-line option to disable the error dialog displayed if the game crashes.
- Improvements for some players using NAT routers. If you're having trouble playing D3 using a NAT, enable port/host forwarding on the NAT server, then specify your port with the the `-useport` and `-pxoport` command-line options.
- Added `-datacheck` command-line option. If you get a message on the loading screen that your mission has data errors, use this option and see the file `datacheck.out` for a description of the data errors in your mission.
- In multiplayer, a HUD message is shown when a player's ship is changed because the selected ship is not allowed.

### Known Issues
- Because of limitations in the precision of Descent 3's timer, high framerates are not displayed accurately on the HUD.