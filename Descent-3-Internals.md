![d3 (1)](https://github.com/DescentDevelopers/Descent3/assets/47716344/8fa6bf0e-0ec0-4130-8fad-fa20bbd93a31)

# Table of Contents
1. [Big Ol' Array](https://github.com/DescentDevelopers/Descent3/wiki/Descent-3-Internals#boa----big-ol-array)
2. [D.A.L.L.A.S.](https://github.com/DescentDevelopers/Descent3/wiki/Descent-3-Internals#dallas----dont-ask-luke-for-levels-and-scripts)
3. [Osiris](https://github.com/DescentDevelopers/Descent3/wiki/Descent-3-Internals#osiris---mission-memory-system)
4. [HOG Files](https://github.com/DescentDevelopers/Descent3/wiki/Descent-3-Internals#hog-files)

# B.O.A. -- Big Ol' Array
This system tells the game what rooms are visible from where--essentially a Potentially Visible Set with some extra features. It may also store pathing costs needed to get from one room to another. `BOA Not Valid!` comes from this and can lead to rendering errors in a level or demo playback. That error is caused by an invalid checksum between the engine and level file--which is in turn due to differences in compilers (specifically, VC6 float math doesn't match current float math).

A band-aid solution is to disable the error message, since invalid BOA just causes the engine to recompute the geometry--pretty quick on modern systems. In reality, a more complete solution is to create a checksum implementation that emulates the original.

# D.A.L.L.A.S. -- Don't Ask Luke for Levels and Scripts
A deprecated visual level scripting system. Generates cpp code. DALLAS could import cpp code inside commented "script blocks" in level scripts for editing. For example, [level4.cpp](https://github.com/DescentDevelopers/Descent3/blob/main/scripts/level4.cpp#L411) has [multiple](https://github.com/DescentDevelopers/Descent3/blob/main/scripts/level4.cpp#L2128) script areas used by DALLAS.

# Osiris - Mission Memory System
Osiris, written by Jeff Slutter, is akin to an API; it reads and manages compiled script libraries. Without scripts, levels become sandboxes where the player can do anything with no guidance. Osiris manages everything in missions from timers, to objects, to objective flags.

# HOG Files
HOG files, short for Hidden Game Object files, are archive format files common in the Descent series and package textures, sounds, levels, and scripts. In Descent 3, the HOG2 format is used. A quick breakdown of the HOG2 format follows:

## HOG Header
The header starts with a 4-byte identifier, set to `HOG2`. Following that is a 32-bit unsigned integer `NFILES`, representing the total number of files included in the hog. Finally, we have the file data offset, a 32-bit unsigned integer representing the offset where actual file data begins. In `HOG2`, file data begins at byte offset 68. After that, there is an array of 56 bytes filled with `0xFF` which serves as reserved header space.

## File Table
Following the header, there's a file table containing information about each file in the hog archive. Each entry here corresponds to a file included in the hog archive and contains metadata, such as the filename, flags, file length, and timestamp.

Each file entry contains the following fields:

- File Name: a 36-byte array representing the name of a file (up to 36 characters)
- Flags: a 32-bit unsigned int representing extra information
- Length: a 32-bit unsigned int representing the length of the file in bytes
- Timestamp: a 32-bit unsigned int

## File Data
Following the file table, the actual file data is stored. Each file's data is stored consecutively after the file table, with each file's data immediately following its corresponding entry in the table.

## Creating HOG2 Files
[WIP]