# Windows

## Installations

`chocolatey` is a package manager for Windows. It is similar to `apt-get` on Linux.

> **Note**: Powershell Core is installed

```powershell
Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://community.chocolatey.org/install.ps1'));
```

> **Note**: `choco` is installed. Restart the terminal to use it.
>
> ***Winget*** is probably installed.

## List of Installed Packages

### Chocolatey

- gh
- ripgrep
- llvm

### Winget

- Google.Chrome
- Google.Drive
- Giorgiotani.Peazip
- Kitware.CMake
- Microsoft.PowerToys
- TheDocumentFoundation.LibreOffice
- OpenJS.NodeJS
- Rustlang.Rustup
- SumatraPDF.SumatraPDF
- GnuWin32.Tar
- VLC media player
- Vivaldi
- OliverSchwendener.ueli
- JanDeDobbeleer.OhMyPosh
- Rainmeter.Rainmeter
- Microsoft.WindowsTerminal
- Git.Git
- Bitwarden.Bitwarden
- msys2.msys2
- Microsoft.VisualStudioCode
- Oracle.JDK.19
- HXAM

### In Script

```powershell
winget install Google.Chrome
winget install Google.Drive
winget install Giorgiotani.Peazip
winget install Kitware.CMake
winget install Microsoft.PowerToys
winget install TheDocumentFoundation.LibreOffice
winget install OpenJS.NodeJS
winget install Rustlang.Rustup
winget install SumatraPDF.SumatraPDF
winget install GnuWin32.Tar
winget install VLC media player
winget install Vivaldi
winget install OliverSchwendener.ueli
winget install JanDeDobbeleer.OhMyPosh
winget install Rainmeter.Rainmeter
winget install Microsoft.WindowsTerminal
winget install Git.Git
winget install Bitwarden.Bitwarden
winget install msys2.msys2
winget install Microsoft.VisualStudioCode
winget install Oracle.JDK.19
winget install HXAM
```

</br>

```shell
choco install gh
choco install ripgrep
choco install llvm
```
