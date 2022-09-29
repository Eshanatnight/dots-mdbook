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
