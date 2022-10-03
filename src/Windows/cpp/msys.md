# MSYS2

MSYS2 should be installed via winget.

In the event that it is not, it can be installed from [here](https://www.msys2.org/).

## Installing/Updating the MSYS2 toolchain

To update the MSYS2-MINGW toolchain just run the following command in the MSYS2 bash shell.

```terminal
pacman -Syu

pacman -S mingw-w64-x86_64-toolchain
```

To update the MSYS2-clang toolchain just run the following command in the MSYS2 bash shell.

```terminal
pacman -Syu

pacman -S mingw-w64-clang-x86_64-toolchain
```

> To update the toolchain use the `-u` flag with the `-S` flag.
