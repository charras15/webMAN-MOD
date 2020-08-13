Git clone # webMAN MOD - Fork of original webMAN plugin by Deank for Playstation 3

__README IS STILL IN PROGRESS, IF YOU SEE ANY ERROR PLEASE TELL ME OR PUSH A COMMIT__

webMAN MOD is a homebrew plugin for PlayStation®3 forked from the original webMAN/sMAN by DeanK
with many features added.


Our goal was to create an AIO plugin that include many of the features available on the PS3 Scene
in an easy and intuitive way. webMAN MOD is the result of the hard work of several users, developers
and artists that collaborated with development, knowledge, resources, feedback & ideas.

## Current functionality
### General
- Support on all custom firmwares with Cobra feature enabled (ver 4.46-4.86 CEX, DEX & DECR)
- Support on REBUG firmware with Cobra feature disabled (ver 4.86.1 CEX & DEX) 
- Support on REBUG firmware with Mamba loaded via boot_plugins_nocobra_kernel.txt (ver 4.86.1 CEX & 4.84.2 DEX) 
- Support on PS3HEN on 4.82 OFW and 4.84-4.86 HFW CEX & DEX
- Support on classic custom firmware with Mamba loaded via IRISMAN (ver 3.41-4.86 CEX & DEX)
- Support on classic custom firmware with Mamba/PRXLoader (ver 3.41-4.86 CEX & DEX)
- Support on classic custom firmware with PRXLoader (ver 3.41-4.86 CEX & DEX)

- All PS3 Models (including all fat, Slim 20xx, 21xx, 25xx, 3xxx & SuperSlims 4xxx) are supported via PS3HEN payload
- All PS3 Models capable to downgrade to 3.56 or lower are supported via PS3Xploit Flash Writer (aka PS3Xploit 2.0)
  See *http://www.psdevwiki.com/ps3/SKU_Models* for compatibility with CFW

### sMAN / webMAN vanilla features
- FTP server with remote control functions (shutdown/restart)
- WWW server with remote control functions (shutdown/restart/mount/cpursx/insert/eject/setup)
- Support for loading and browsing of [local] PS3 games in ISO and folder format, DVD videos in ISO format, Blu-ray movies in ISO format, PS1/PS2/PSP games in ISO format with cover display
- NETISO support for network loading and browsing of PS3 games in ISO and folder format, DVD videos in ISO format, Blu-ray movies in ISO format, and PS1 games in ISO format.
- NTFS support for PS3 and PS1 games in ISO format, Blu-ray movies in ISO format and DVD Video in ISO format
- Manual and Dynamic Fan Control and in-game temperature monitoring
- PAD shortcuts (*open include/combos.h for a complete list of shortcuts)
- Keep external USB device alive & Reset USB Bus
- Mount last game or AUTOBOOT.ISO to system startup
- Support direct access to NTFS devices through web & ftp (1.45 / 1.45.11)
- XMB integration XMB proxy (1.46 / 1.46.00)
- Integrated prepNTFS (1.47)

### webMAN MOD additional & extended features

#### Installer & GUIs
- Easy installer/updater with 4 editions: full, lite, standard (rebug) & nonCobra.
- New icons created by Brunolee & Berion
- VSH Menu integration (hold SELECT to show the menu)
- sLaunch GUI integration (hold START or R2+L2 on XMB to show the game menu GUI)
- Coverflow web-GUI (/games.ps3) provides a mobile/desktop friendly GUI for fast selection of games.
- Grid web-GUI (/index.ps3) display games with resizable icons and content can be filtered by type/device/name
- 2 GUI Themes: sMAN-like graphical interface & webMAN original theme
- LaunchPad integration (DeViL303' mod to use What's New section to mount games)
- PhotoGUI integration (DeViL303' mod to use Photo albums to mount games)
- XMBM+ integration when grouping of XMB content is disabled (v1.33.03)
- Support for custom XML menu integrated into webMAN Games menu
- Install packages from any folder using web command: /install.ps3<path>

#### Localization & Regional settings
- Translated into 23 languages
- Support for change BD/DVD region

#### Content organization & information display
- Title ID can be displayed on XMB menu
- Covers are shown using the Title ID found in the file name of the ISO or folder name (JB game).
- Option for display original file name or title name from PARAM.SFO
- Option for display covers as discs, ICON0.PNG or covers from multiMAN, IRISMAN, ManaGunZ repository or in the same folder of the ISO
- Option for online covers display (free service provided by DeViL303)
- Optional Video subfolder to "Bluray™ and DVD" folder (Display RetroXMB videos, videos on USB devices and Data Disc icon)
- Extended system information via /cpursx.ps3 (Title ID, game icon, APP Version, IDPS/PSID, CFW version, last played game, console's run time & number of boots)
- Display of Play time & startup time to SELECT+START and /cpursx.ps3 (Use SELECT+START+R2 to display Game ID, Title, play time and more in-Game info)
- Use "home" path to define default path for /app_home/PS3_GAME on start up and for R2+START (e.g. make app_home start multiMAN or IRISMAN)
- Support for list NPDRM games stored /dev_hdd0/game in addition to ISO and JB folders
- Support for exclude games by file name & Title ID using wm_ignore.txt

#### Extended mount of game
- It can mount PSP games stored on exFAT/ext/NTFS/NET devices without copy the file to the internal HDD (1.47.27) - Requires prepISO 1.27 or later
- It can mount PS2 Classics games on PS2 Classic Launcher (.BIN.ENC)
- Automatic CONFIG creation for PS2ISOs and PS2 Classic using config database from ManaGunZ or the database of CONFIG created by the installer
- Support for launch SELF applications via PKG/ROM Launcher or through the XMB icon: ★ app_home/PS3_GAME
- Integrated external gameDATA allows installation of packages & game data on external USB drives
- Integrated prepNTFS allows to scan PS3ISO, PSXISO, BDISO & DVDISO on NTFS devices without require prepISO/prepNTFS
- Support for *.ntfs[BDFILE]* (fake ISO created by IRISMAN or prepISO/prepNTFS) - Used to play movies or install large packages on NTFS
- Support to mount NTFS games using raw_iso.sprx (rawseciso by Estwald) - Supports fake ISO
- Support last_game.txt / autoboot on nonCobra edition
- Auto install PKG mounted from exFAT/ext/NTFS (reduce steps needed to install a PKG)

#### Emulation features
- ROMS support through PKG/ROM Launcher and RetroArch (support internal HDD/USB/NET storage with custom icons & background images)
- Enable selection of emulator for PS1 and PS2 on B/C consoles
- PS2 Launcher / PSP Launchers can be integrated into webMAN Games menu for easy access

#### File management & navigation
- Improvements on File Manager (file & folder icons, links to navigate faster, mount ISO, mount net0/ or net1/, preview images, copy/paste/delete files & folders)
- Copy operations use shadow copy on hdd0 for faster copy operations
- It can rip a game from disc to hdd0 or copy from hdd0 to usb000 or from usb00x to hdd0.
- Shorter URL to access paths & files. Use "home" path for search in a user defined folder.
- Support for MD5 hash verification of files stored on PS3 (internal HDD & USB FAT32 only)
- Support edition of small text files (up to 1,300 bytes) via web
- Hex File Viewer (internal HDD/FAT32/NTFS)

#### Network features
- PS3 Manager API Support (PS3MAPI) compatible with RTM tools
- FTP server includes new SITE commands to allow copy/paste files locally, unmount game, toggle external gamedata, turn on/off dev_blind, change file attributes
- Extended support up to 5 remote network servers
- Auto configure remote IP address when /setup.ps3 is accessed from a remote client
- Support navigation of remote network servers even if they are disabled for content scanning
- NETISO server on PS3 (ISO only) lets share local games among PS3 consoles in a LAN
- Download files & install PKG remotely or with pad shortcuts
- /dev_blind and /dev_hdd1 are auto-mounted when accessed via FTP or http
- Support for local web chat (source code only)

#### Automatization
- Support for user defined combos (pad shortcuts)
- Virtual pad allows send button events remotely via http://pad.aldostools.org on web browser or with webPAD software (Windows only)
- Support for auto-play on startup any supported ISO, game folder or auto-open an URL link. webMAN vanilla only can mount AUTOBOOT.ISO
- Several shortcuts to toggle Cobra, swap Rebug files, mount net0/ or net1/, show IDPS/PSID, etc.
- Support for auto-fix games that require higher FW version (4.20 and later)
- Support batch script automation at startup (dev_hdd0/boot_init.txt or dev_hdd0/autoexec.bat) or played at any time (/play.ps3/<script-file>.bat)
- Launch mounted games with /play.ps3 command. Once a game is mounted via html, click on the displayed icon to launch the game on the PS3.
- Execute XMB functions with /play.ps3 command. (e.g: /play.ps3?col=network&seg=seg_premo) <- this will start Remote Play server from XMB.
- A comprehensive set of web commands and features for customization (link in Web Commands Documentation)

#### Stealth features
- Support for dumping IDPS/PSID
- Support for automatic or manual removal of CFW syscalls and spoof console id (IDPS/PSID)
- "Offline" mode (blocks some PSN/tracking servers) and automatic restore when CFW syscalls are removed. Game updates still work in this mode. (v1.33.03)
- Scan for games on the stealth folder "/video"
- Auto unlock savedata during download & copy operations (removes account id, PSID & copy protection

#### Safety & security features
- Improved temperature monitoring (max & min fan speed, auto#2 mode, improved algorithm for dynamic fan control)
- Increased security: ADMIN mode blocks access to critical functions like /setup.ps3, /delete.ps3; Password for FTP server access; limit remote access to specific IP
- dev_bdvd/PS3_UPDATE is redirected to prevent an accidental update if a game disc is inserted in the drive
- Extended Content Profile Grouping (v1.33.07) - common files + individual content (4 profiles)
- Safe upload mode prevents a brick/semi-brick if power fails during ftp uploads to /dev_blind.

#### Memory & debugging
- All LV2 peek/pokes are done through syscalls 8/9 (CFW only) - syscalls 6/7 used only by PS3HEN
- Web Debugger (remote peek/poke/find bytes, dump lv1 & lv2 memory)
- MIN+ memory profile (same as MIN but uses 512K and 2.5X more buffer for PS3 games)
- MAX+ memory profile (same as MAX 1280K for PS3 games, others buffer is reduced, eg: 2X less buffer for ftp and 4X for DVD etc...)
- Support for up to 3MB from 4 available memory containers (bg, fg, debug, app)
- Remote syscalls

#### Screen & video capture
- Capture XMB screen in BMP format
- Enable in-game screen capture on CFW that don't has the feature.
- Integrated Mysis video_rec plugin and get klicensee used by NPDRM content

## Web Commands Documentation
https://www.psx-place.com/threads/webman-mod-web-commands.1508/

## Integrated Plugins
- sLaunch plugin : GUI to navigate and mount the games from any place on the XMB
- VSH Menu plugin : GUI to execute commands from any place on the XMB
- RAWSECISO plugin : Proxy that handles the SCSI requests by Cobra to access the ISO images stored in exFAT/NTFS devices
- NETISO plugin : Proxy that handles the SCSI requests by Cobra to access content stored in the remote servers (ps3netsrv)
- Video REC plugin : Standalone plugin that records video from games. When used, webMAN MOD is unloaded to free memory.

## Addons
- ps3netsrv : Remote content distribution server for PC and linux platforms that uses Cobra's NETISO protocol for streaming of content
- prepISO : tool that scans content stored in exFAT / NTFS devices and prepare the settings files needed by RAWSECISO plugin
- PKG/ROM Launcher : allows the execution of PS3 applications and ROMS via RetroArch. Requires that the debug icon "★ app_home/PS3_GAME" be present on XMB
- PS2CONFIG : Database of PS2 CONFIG files needed to improve the compatibility of certain PS2 games
- WM Themes : Set of packages that customize the look of the XMB icons used by webMAN MOD
- Reload XMB : PS3 application that forces the reload of XMB icons
- Boot MAMBA : Package that installs MAMBA payload for use on Rebug 4.84 and later with Cobra disabled
- MOVIAN.ISO : Custom ISO to launch MOVIAN

- PS2 Classics Launcher : PS3 application required to launch PS2 Classics games in .BIN.ENC format
- PSP Remasters Launcher : PS3 application required to launch PSP Remaster games in ISO format
- PSP Minis Launcher : PS3 application required to launch PSP Mini games in ISO format

- RetroArch : Required to launch the emulators that run the classic games in ROM format
- MOVIAN : Required to play audio and videos in non-nantive formats

- webPAD : http://pad.aldostools.org - Online virtual game pad

## How to build
Requirements for Windows:
- git, clone this repository with the following command: *git clone https://github.com/aldostools/webMAN-MOD.git*
- Official PS3 SDK v3.40 or 4.00 complete leaked version, google is your friend to find it
- GCC (for Windows [MinGW](http://sourceforge.net/projects/mingw) with mingw32-base will be fine) or [Cygwin (x86/x64)](https://cygwin.com/install.html)
- Open Source PSL1GHT SDK to compile prepISO and PKG Updater only

Requirements for GNU/Linux:
- An x86 linux distribution, Fedora 20 is tested working
- git, clone this repository with the following command: *git clone https://github.com/aldostools/webMAN-MOD.git*
- Official PS3 SDK v400.001 leaked version
- Official Cell OS Lv-2 leaked toolchain (a 4.1M patched GCC 4.1.1 version)
- wine for the missing linux tools
- A compiled Scetool binary, ps3 keys
- Open Source PSL1GHT SDK to compile prepISO and PKG Updater only

## Credits
- All the documentation on *http://www.psdevwiki.com*, and to all the devs who contributed
- Cobra team, for their work on Cobra payload and sharing the source code in public (thanks to the request of STLcardsWS)
- Deank as the creator of webMAN, sMAN, sLaunch, multiMAN / mmCM and many other contributions to the scene
- Estwald for NTFS library, rawseciso, fake iso, Mamba payload, etc.
- Aldo Vargas (aldostools) for all his works on this project!
- Zar & m@tsumot0 for starting the modding project
- NzV for PS3 Manager API (aka PS3MAPI), Mamba/PRX Loader & Mamba improvements
- bguerville for ps3xploit, tools, web downloader & package installer modules and port of ntfslib
- The team that ported NTFS library from PSL1ght to PS3 SDK (freddy38510, bguerville, Zar, deank, Joonie)
- Mysis, who wrote some useful libs and reverse engineering VSH Exports functions: http://www.ps3devwiki.com/ps3/VSH#Exports
- 3141card for VSH Menu POC & Littlebalup for his enhancement/new features
- jjolano (John Olano) for OpenFTP server
- OsirisX for PS3XPAD and the source code needed for gamepad emulation
- Berion & Brunolee for the graphics & icons
- bucanero port of libraries for zip, rar, 7zip
- lmirel port of libraries for exFAT
- PSX-SCENE, PSX-PLACE, PLAYSTATIONHAX, PS3HAX & other scene websites/users, who translated, helped in the testing process

Special thanks to Joonie, Habib & Rebug Team, flatz, haxxxen, devil303, Rancid-O, EvilNat, KW, naehrwert, MiralaTijera


## License
### webMAN MOD

webMAN MOD is a FREE software and all its components (ps3netsrv included) are
distributed and protected under GNU General Public License version 3 (GPL v3)
as published by the Free Software Foundation, or (at your option) any
later version..

That means that any change made to the source code, binaries or resources
of this software must be made public. A detailed list of the changes and
the credits to the original authors are strictly required.

It is NOT permitted to distribute modified versions with the same name
of this software. A similar name or misleading name should NOT be used,
to avoid confusion about the origin or the version in use.

For futher information about GPL v3, refer to:
https://www.gnu.org/licenses/gpl-3.0.en.html

THE SOFTWARE IS DISTRIBUTED "AS IS". NO WARRANTY OF ANY KIND IS EXPRESSED
OR IMPLIED. YOU USE AT YOUR OWN RISK. NEITHER THE AUTHOR, THE LICENSOR NOR
THE AGENTS OF THE LICENSOR WILL BE LIABLE FOR DATA LOSS, DAMAGES, LOSS OF
PROFITS OR ANY OTHER KIND OF LOSS WHILE USING OR MISUSING THIS SOFTWARE OR
ITS COMPONENTS. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE
FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE
OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

Furthermore, the author and his ASSOCIATES shall assume NO responsibility,
legal or otherwise implied, for any misuse of, or for any loss of any kind
that may occur while using the SOFTWARE or its components.

Installing and using the software signifies acceptance of these terms and
conditions of the license. If you do not agree with the terms of this license,
you must remove all software files from your storage devices and cease to use
the software.



(C) 2010-2020 multiMAN / webMAN by DeanK

Permission is hereby granted, free of charge, to any person
obtaining a copy of this software and associated documentation files
(the "Software"), to deal in the Software without restriction,
including without limitation the rights to use, copy, modify, merge,
publish, distribute, sublicense, and to permit persons to whom
the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be
included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS
BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN
ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
