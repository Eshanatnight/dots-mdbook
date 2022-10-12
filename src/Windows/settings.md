# Settings

## Configuration Files

The Settings files can be found

[Visual Studio Settings](https://github.com/Eshanatnight/dotfiles/blob/main/.visual-sutdio-settings/.vs.settings.tar.gz.tar.gz?raw=true)

[Visual Studio Extentions](https://github.com/Eshanatnight/dotfiles/blob/main/.visual-sutdio-settings/vs-extention.tar.gz?raw=true)

[Jetbrains](https://github.com/Eshanatnight/dotfiles/tree/main/.jetbrains-settings)

## Jetbrains

### Configure a WSL Toolchain

1. In CLion, go to Settings / Preferences | Build, Execution, Deployment | Toolchains.

2. Click plus icon to create a new toolchain and select WSL.

3. In the Environment field, select one of the available WSL distributions. The list includes the distributions detected by wsl.exe --list, which includes the imported ones.

4.Now to start using the toolchain, do the following:

- CMake
- Makefile
