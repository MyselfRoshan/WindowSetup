# Install Window without any debloat

## Download the Windows.iso and create installation media.

`Step 1 :` Click the links below to download official Windows ISO :

- [Windows 10](https://www.microsoft.com/software-download/windows10)
- [Windows 11](https://www.microsoft.com/software-download/windows11)

`Step 2 :` Create bootable USB drive using program metioned below :

- [Ventoy](https://www.ventoy.net/en/download.html) (Recommended)
- [Etcher](https://www.balena.io/etcher) (Beginner Friendly)
- [Rufus](https://rufus.ie/en/)

## Some famous debloating scripts (Recommended)

```powershell
irm -useb https://christitus.com/win | iex
```

```powershell
irm -useb https://git.io/debloat | iex
```

## Install Enterprise LTSC version of windows without any bloat

## Install winget, choco, scoop packet manager (Optional)

_`Note: Use Ctrl+V within Powershell(with Administrator) to run all code at once`_

`Step 1 :` To install winget without Microsoft Store

```powershell
Set-PSRepository -Name 'PSGallery' -InstallationPolicy Trusted
Install-Script -Name winget-install -Force
winget-install.ps1
```

`Step 2 :` To install choco

```powershell
Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://community.chocolatey.org/install.ps1'))
```

`Step 3 :` To install scoop

```powershell
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
irm get.scoop.sh | iex
```

## Some of the system utility tools

- [Tron](https://github.com/bmrf/tron) - An automated PC cleanup script **(RECOMMENDED)**
- [Kasperky Rescue Disk](https://www.kaspersky.co.in/downloads/free-rescue-disk)
- [Kasperky Virus Removal Tool](https://www.kaspersky.co.in/downloads/free-virus-removal-tool)

## Some of the recommended software

- [qbittorrent](https://www.qbittorrent.org/download) - A free and reliable P2P BitTorrent client in C++ / Qt that uses libtorrent (sometimes called libtorrent-rasterbar) by Arvid Norberg
- [f.lux](https://justgetflux.com/) - Alternative to Windows nightlight with various options
- [ShareX](https://getsharex.com/) - Alternative to windows Snipping tools for taking screenshots, record screen, pick colors,etc.
