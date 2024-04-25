![d3 (1)](https://github.com/DescentDevelopers/Descent3/assets/47716344/8fa6bf0e-0ec0-4130-8fad-fa20bbd93a31)

# Table of Contents
1. [Big Ol' Array](https://github.com/DescentDevelopers/Descent3/wiki/Descent-3-Internals#boa----big-ol-array)
2. [D.A.L.L.A.S.](https://github.com/DescentDevelopers/Descent3/wiki/Descent-3-Internals#dallas----dont-ask-luke-for-levels-and-scripts)
3. [Osiris](https://github.com/DescentDevelopers/Descent3/wiki/Descent-3-Internals#osiris---mission-memory-system)

## B.O.A. -- Big Ol' Array
This system tells the game what rooms are visible from where--essentially a Potentially Visible Set with some extra features. It may also store pathing costs needed to get from one room to another. `BOA Not Valid!` comes from this and can lead to rendering errors in a level or demo playback.

## D.A.L.L.A.S. -- Don't Ask Luke for Levels and Scripts
Visual level scripting system. Generates cpp code. DALLAS could import cpp code inside commented "script blocks" in level scripts for editing. For example, [level4.cpp](https://github.com/DescentDevelopers/Descent3/blob/main/scripts/level4.cpp#L411) has [multiple](https://github.com/DescentDevelopers/Descent3/blob/main/scripts/level4.cpp#L2128) script areas used by DALLAS.

## Osiris - Mission Memory System
Osiris, written by Jeff Slutter, is akin to an API; it reads and manages compiled script libraries. Without scripts, levels become sandboxes where the player can do anything with no guidance. Osiris manages everything in missions from timers, to objects, to objective flags.