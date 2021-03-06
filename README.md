# cso2-launcher

[![Build status](https://ci.appveyor.com/api/projects/status/ajl6d1ir9s3l4lyu/branch/master?svg=true)](https://ci.appveyor.com/project/Ochii/cso2-launcher/branch/master)

**This user is only a proof of concept that you can host your own match, it does not emulate every game feature.**

You can use this to start a game match in Nexon's (South Korea) Counter-Strike: Online 2.

If you wish to see the client that connects to an emulated server, go [here](https://github.com/Ochii/cso2-launcher/tree/server_emulator).

## Download 
You may download the latest build of it **[here](https://github.com/Ochii/cso2-launcher/releases/latest)**.

## How to use
**This tool requires a copy of Nexon's Counter-Strike: Online 2.**

You may get one [here (MEGA)](https://mega.nz/#!nhgnBJgD!iR57D5Mf3_1GCcAR36tqFQ7H7KN_F0e3XicD2JBoSN4) or [here (Google Drive)](https://drive.google.com/open?id=1y0diL2nTERlOaJZQTA3xPb8owx82GjtB) (SHA-256: 02F76DBDD083EF78ECC92EB963C7C7A7576FF2E2C695671A4F358C2580584965).

[Download](https://github.com/Ochii/cso2-launcher/releases/latest) the tool archive file, then extract its contents inside ```[your CSO2 game path]/Bin```.

To play, start ```launcher_main.exe```. When in the login menu, you may input the following commands in the console.

### Console commands
- ```joinroom [gamemode id] [map id]``` - Creates a room and starts the room match
- ```listgamemodes``` - Lists the available game modes
- ```listmaps``` - Lists the available maps
- ```lessdebug``` - Shortens the information printed in the console

Some useful ingame commands:

- ```jointeam [team number]``` - Joins you in a team, where 1 is spectator, 2 is terrorist and 3 is counter-terrorist
- ```disconnect``` - Disconnects you from your current match

You may also use this console as if it was an ingame console (you can enable ```cl_showfps```, for example).

## Bug reporting and improvements
Have a look at the [issues](https://github.com/Ochii/cso2-launcher/issues) for a list of bugs found or to report them yourself.

If you have any improvements that you would like to share, go ahead and [open a pull request](https://github.com/Ochii/cso2-launcher/pulls).

## How to build

### Requirements
- [CMake](https://cmake.org/download/)
- [Visual Studio 2017](https://www.visualstudio.com/downloads/)
- [Windows PowerShell](https://docs.microsoft.com/en-us/powershell/scripting/setup/installing-windows-powershell)

Only **Windows** is supported.

### Downloading the source code
Clone the project with ```git clone --recursive https://github.com/Ochii/cso2-launcher.git```.

### Before building
Start a PowerShell instance and change directory to the project's directory, then, run ```./setuplibs.ps1```.

The script will setup PolyHook, its dependency Capstone and the Source SDK.

### Building
Open the solution ```CSO2Launcher.sln``` and build it in your preferred configuration.

If built successfully, you will find your binaries inside ```out/bin/Win32/[your configuration]```.

## Used libraries
- **[PolyHook](https://github.com/stevemk14ebr/PolyHook)** by [stevemk14ebr](https://github.com/stevemk14ebr)
- **[Capstone](https://github.com/aquynh/capstone)** by [aquynh](https://github.com/aquynh/capstone)

## Credits
- [Valve Software](https://github.com/ValveSoftware/source-sdk-2013) for their SDK

## Thank you's (by no particular order)
- To **[UserU](https://www.youtube.com/user/GoodbyeSpy)**
- To **[SHI_KU](https://www.youtube.com/channel/UC2HZo-HFOuxmS6zWYPMD0hQ)**
- To **ReddUT** from [Counter-Strike Online Wikia](https://cso.wikia.com/)'s Discord
- To **Frostie** from [Counter-Strike Online Wikia](https://cso.wikia.com/)'s Discord 

## License
Read ```LICENSE``` for license information.

I'm not affiliated with either Valve or Nexon, just like I don't own Counter-Strike Online 2.
