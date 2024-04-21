# Table of Contents
1. [System Requirements](https://github.com/DescentDevelopers/Descent3/wiki/Running-Descent-3#system-requirements)
2. [Command-Line Options](https://github.com/DescentDevelopers/Descent3/wiki/Running-Descent-3#command-line-options)

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
The following command-line options are available in Descent 3. You can set command-line options on the Misc. tab of the Setup section of the Descent 3 launcher. Case is not significant in command-line options.

**Display Options:**
- `-aspect <value>`: Specifies the screen aspect ratio for non-standard displays, such as wide-screen TVs.
- `-height <height>`: Sets the screen resolution to the specified height, if possible.
- `-himem`: Forces normal operations even when low memory conditions are detected.
- `-lowmem`: Uses scaled-down textures and lower quality (8-bit) sounds to conserve memory.
- `-NoRenderWindows`: Causes all windows to be fully transparent. Use this option if your card does not correctly render partially-transparent windows.
- `-superlowmem`: Uses the `-lowmem` settings and further scales down textures to conserve memory.
- `-vsync`: Turns on Vertical Sync. The flag will be enabled in the registry so it will be on when the game is run again.
- `-width <width>`: Sets the screen resolution to the specified width, if possible.
- `-windowed`: Runs the game in a window.
- `-z32bit`: Enables the 32-bit z-buffer on cards that support it, such as the Matrox G400.

**Audio Options:**
- `-nomusic`: Disables music.
- `-nosound`: Disables all sound, including music.

**Controls Options:**
- `-alternatejoy -directinput`: Causes DirectInput to be used for the joystick or other game controller, instead of standard Windows API.
- `-chpro`: Enables a CH Flightstick Pro or compatible joystick.
- `-deadzone# <k>`: Specifies the size of the deadzone for a joystick.
- `-mlooksens <scale>`: Determines how much the player moves when the mouse is moved.
- `-mouseman`: Enables special handling for the Logitech MouseMan.
- `-mousesens <scale>`: Adjusts the sensitivity of the mouse when not using mouselook mode.

**Multiplayer and Network Options:**
- `-audiotauntdelay <time>`: Sets the time in seconds the a user must wait after sending an audio taunt before he or she is able to send another. This option is only active when starting a server.
- `-autoexec <file>`: Specifies the full path and file name of the multiplayer config file to be loaded and executed when a multiplayer game is initialized.
- `-dedicated <config file>`: Starts a dedicated server.
- `-gamespyport <port>`: Specifies a port for to listen for GameSpy requests. The default is 20142.
- `-gspyfile <config file>`: Specifies a GameSpy configuration file to use (default is gamespy.cfg).
- `-httpproxy <addr>` or `-httpproxy <addr:port>`: Specifies an HTTP proxy server. Descent 3 uses HTTP to auto-download a mission; use this option if your ISP requires a proxy server for HTTP connections. If the first form is used, the port value defaults to 80.
- `-nooutragelogo`: Disables the Outrage logo that is normally displayed for five seconds at the start of a multiplayer game.
- `-nomultibmp`: Disables sending or receiving in-game custom bitmaps for ships.
- `-nonetwork`: Disables all network multiplayer functionality.
- `-playermessages`: Disables all weapon-related HUD messages in multiplayer games.
- `-pxoport <port>`: Specifies the port that PXO will tell clients to use when contacting a server. The default is 2092.
- `-useip <IP>`: Binds Descent 3 to this IP address. Use this option to tell D3 which IP address to use if your computer has multiple IP addresses.
- `-useport <port>`: Specifies the port that TCP/IP and IPX will use. The default is 2092.
- `-usesmoothing`: Enables code to smooth the interpolation for fast-moving objects. This will fix "skipping" problems with fast weapons, such as the Phoenix. This option applies to clients only; using it on the server has no effect.


**Other Options:**
- `-fastdemo`: Causes a demo to play back at the highest speed your computer is capable of.
- `-forcelightmaps`: Forces the use of lightmaps, even the Default Detail Level is set to Low in the launcher setup.
- `-framecap <fps>`: Limits the framerate to the number of frames per second specified.
- `-highvidmem`: Causes 2 MB Voodoo 1 cards to behave as if they had more memory.
- `-makemovie`: Causes the demo system to save a screenshot of every frame during playback.
- `-mission <name>`: Loads the specified mission file at startup.
- `-nocompress`: Turns off S3TC texture compression for cards that support it.
- `-nocrashbox`: Disables the error dialog displayed if Descent3 crashes.
- `-nopentium3`: Disables detection of the Pentium III processor.
- `-nomotionblur`: Disables motion blur on robots (Pentium III only).
- `-nosatomega`: Disables alpha saturation on the omega cannon effect.
- `-nosparkles`: Disables powerup sparkles (Pentium III only).
- `-setdir <path>`: Specifies the working directory for Descent 3.
- `-timetest <file>`: Causes Descent 3 to play back the specified demo file upon startup.
- `-useexedir`: Tells Descent 3 to use the directory in which the executable is located as the working directory.