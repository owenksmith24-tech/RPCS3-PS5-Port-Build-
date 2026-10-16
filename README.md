# RPCS3-5-Disk-Support

# RPCS3-5

RPCS3, the PS3 emulator, running natively on jailbroken PS5 consoles. It plays PS3 discs straight from the PS5's disc drive.

Built on [KB-RPCS3](https://github.com/kamb205/KB-RPCS3) v0.1.0-alpha. Latest: **v1.2.2 Beta**.

## Features
- Plays PS3 discs from the PS5's drive (Redump keys come as a separate download), as well as `.iso` files, game folders and PSN `.pkg` files
- The PS5 ejects the disc normally after you play, with no console restart
- Per-game settings
- One-command installer that works over the PS5 Upload app or FTP, with any console IP
- Diagnostic tools: helper and disc probes, log and FPS readers

## Tested
| Game | Status |
|---|---|
| Call of Duty: World at War (BLUS30192) | Plays |
| Call of Duty: Modern Warfare 3 (BLUS30838) | Plays at 1280x720, mostly 45–60 FPS |

Tested on a PS5 Slim, firmware 13.60.

## Requirements
- A jailbroken PS5
- etaHEN
- kstuff lite
- ShadowMountPlus
- Your own `PS3UPDAT.PUP`

## Install
1. Download both zips from Releases, put them in one folder and extract the app zip there.
2. Open the PS5 Upload app and connect it to the PS5, or turn on etaHEN's FTP server (port 1337).
3. Run `.\Install-RPCS3-5.ps1 -Ps5 <PS5 IP>` in PowerShell.
4. On the PS5, go to RPCS3-5 > Install > PS3 firmware. Then, in Settings, set Clocks scale to 100 and Frame limit to Auto.

## Notes
- Swap discs only from the RPCS3-5 home screen.
- Call of Duty games: set the in-game resolution to 1280x720.
- This is beta software. Use it on your own consoles only and don't redistribute builds: KB-RPCS3's author asks this because the GPL-2.0-only RPCS3 core is combined with GPL-3.0 components.

## Credits
kamb205 (KB-RPCS3) · RPCS3 team · Mihawk (PS5 Vulkan driver, Mesa, payload SDK, LLVM)
