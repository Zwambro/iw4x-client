![license](https://img.shields.io/github/license/IW4x/iw4x-client.svg)
![forks](https://img.shields.io/github/forks/IW4x/iw4x-client.svg)
![stars](https://img.shields.io/github/stars/IW4x/iw4x-client.svg)
![issues](https://img.shields.io/github/issues/IW4x/iw4x-client.svg)
[![build status](https://ci.appveyor.com/api/projects/status/rvljq0ooxen0oexm/branch/develop?svg=true)](https://ci.appveyor.com/project/iw4x/iw4x-client/branch/develop)
[![discord](https://discordapp.com/api/guilds/219514629703860235/widget.png)](https://discord.gg/sKeVmR3)

# IW4x: Client

## Commit message style

```
[Module] Imperative summary

- points or text

[ci skip]
```

`[ci skip]` is optional.

## How to compile

- Run `premake5 vs2019` or use the delivered `generate.bat`.
- Build via solution file in `build\iw4x.sln`. (You can use the `build.bat` script to do it quick and easy.)

## Premake arguments

| Argument                    | Description                                    |
|:----------------------------|:-----------------------------------------------|
| `--copy-to=PATH`            | Optional, copy the DLL to a custom folder after build, define the path here if wanted. |
| `--copy-pdb`                | Copy debug information for binaries as well to the path given via --copy-to. |
| `--ac-disable`              | Disable anticheat.                             |
| `--ac-debug-detections`     | Log anticheat detections.                      |
| `--ac-debug-load-library`   | Log libraries that get loaded.                 |
| `--force-unit-tests`        | Always compile unit tests.                     |
| `--force-exception-handler` | Install custom unhandled exception handler even for Debug builds. |
| `--force-minidump-upload`   | Upload minidumps even for Debug builds.        |
| `--disable-bitmessage`      | Disable use of BitMessage completely.          |
| `--disable-base128`         | Disable base128 encoding for minidumps.        |
| `--no-new-structure`        | Do not use new virtual path structure (separating headers and source files). |
| `--enable-dxsdk`            | Enable DirectX SDK (required for GfxMap exporting). |

## Disclaimer

This software has been created purely for the purposes of
academic research. It is not intended to be used to attack
other systems. Project maintainers are not responsible or
liable for misuse of the software. Use responsibly.
