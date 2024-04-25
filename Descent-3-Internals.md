# [WIP] Descent 3 Internals
This page explains terminology seen in the source code and hopes to inform how the game engine works.

## B.O.A. -- Big Ol' Array
This system tells the game what rooms are visible from where--essentially a Potentially Visible Set with some extra features. It may also store pathing costs needed to get from one room to another. `BOA Not Valid!` comes from this and can lead to rendering errors in a level or demo playback.

## D.A.L.L.A.S. -- Don't Ask Luke for Levels and Scripts
Visual level scripting system. Generated cpp code. DALLAS could import cpp code inside commented "script blocks" in level scripts for editing. For example, [level4.cpp](https://github.com/DescentDevelopers/Descent3/blob/main/scripts/level4.cpp#L411) has [multiple](https://github.com/DescentDevelopers/Descent3/blob/main/scripts/level4.cpp#L2128) script areas used by DALLAS.

## Osiris - Mission Memory System
Osiris, written by Jeff Slutter, is akin to an API; it reads and manages compiled script libraries. Without scripts, levels become sandboxes where the player can do anything with no guidance. Osiris manages everything in missions from timers, to objects, to objective flags.