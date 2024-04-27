![image](https://github.com/DescentDevelopers/Descent3/assets/47716344/a772b8e6-4b2f-4606-aa3f-35208189d11b)

# Weekly Summary: Apr 22 - Apr 27 2024

Repository Improvements:
- Created wiki pages for `Descent 3 Internals`, `Running Descent 3`, and `Weekly Updates`.
- Added new issue and pull request templates.
- Prettified the readme.
- The CI no longer runs if no changes are made to code (can be manually run).

Bug Fixes:
- Main menu now properly renders if `mainmenu.mve` is missing.
- Descent 3 no longer prompts for a CD if movies aren't found.
- A sanity check was added for when an object is already unlinked from a room, which fixed crashes on Linux.
- A crash where the engine would try to play a sound from an unlinked object was fixed.
- An audio crash on 64-bit platforms was fixed in `libacm`. Thanks DanielGibson and Winterheart for the troubleshooting!
- An audio cutoff issue was fixed in `libacm`.
- A checksum failure caused level scripts to fail loading on 64bit builds. This is fixed by forcing the valid 64bit checksum on 64bit builds.
- A bug where controls were broken on AMD processors was fixed.


Adjustments:
- Console logging enabled on Mac and Linux with `-D LOGGER=ON` cmake option (added to readme).
- The `-windowed` command-line option has been disabled on Release builds.
- The game now links against the real zlib. This introduced a new dependency, and the build instructions were updated as a result.
- The game window in Debug mode can now be dragged around. However, this introduces a bug. See Known Issues.

Known Issues:
- The hardware cursor is still active in `-windowed` mode, which can cause focus loss problems when firing weapons.
- The MacOS build doesn't capture the mouse, making the mouse unusable. Use the magic keypress `Ctrl+Shift+G` to capture the mouse after loading a level as a workaround. We are working on a solution.

General Updates:
- Ryan C. Gordon aka Icculus was given approval to add his code changes from the 2020 linux/mac port. This is an ongoing process and not all code may be merged.
- We are waiting for clarification before replacing libmve. When the repository first went up, the readme stated proprietary Interplay mve code was removed. We were later told libmve would need to be replaced.
- Discord user icecoldduke has been working on the internal editor. We are hoping to bring this upstream after testing it so we can have it compile together with Descent3.
- A multiplayer server is live at `64.44.131.41`. Thanks DescentMax7930 for hosting!
- [Issue #193](https://github.com/DescentDevelopers/Descent3/issues/193) shows Direct3D render enhancements that OpenGL does not have. Pending libmve and other short-term roadmap options, we have yet to talk about whether this should move up on the priority list.
