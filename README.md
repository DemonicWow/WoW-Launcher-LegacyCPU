# Arctium Game Launcher (Public version)
A game launcher for World of Warcraft that allows you to connect to custom servers with a valid tls certificate attached.

**NOTE**: This is a publicly available, stripped down version of the launcher. The **full-featured** launcher is distributed under different terms and is available at https://arctium.io

### License, Copyright & Contributions

Please see our Open Source project [Documentation Repo](https://github.com/Arctium/Documentation)

## Special Request <3
Please do NOT remove the name `arctium` from the final binary.
Blizzard filters their crash logs based on localhost and the string `arctium` in the binary name. 

### Supported Clients
* 1.14.4 or later
* 3.4.2 or later
* 10.1.5 or later

**Later = all future version in that branch.**

### NOTE FOR SERVER CONNECTIONS
* A valid certificate matching your authentication/bnet server host name.
  That certificate needs to be loaded by the authentication/bnet server too

### Binary Releases
There are no binary releases of this version. Our **full-featured** launcher has binary releases at https://arctium.io

## Building

### Build Prerequisites
* [.NET Core SDK 10.0.0 or later](https://dotnet.microsoft.com/download/dotnet/10.0)
* Optional for native builds: C++ workload through Visual Studio 2026 or latest C++ build tools

### Build Instructions Windows (native)
* Execute `dotnet publish -r win-x64 -c Configuration -p:platform="x64" -p:PublishAot=true`
* Native output is placed in the `build` folder.

## Usage

### Windows Usage
1. Copy `Actium Game Launcher.exe` to your World of Warcraft folder.
2. Edit the `WTF/Config.wtf` to set your portal or use a different config file with the `-config Config2.wtf` launch arg.
3. Run the `Actium Game Launcher.exe`

### Launch Parameters
Use `--help`
