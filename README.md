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
irm https://christitus.com/win | iex
```

```powershell
irm https://git.io/debloat | iex
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

_`Note : If you face any problem with winget execute the following commands:`_
```powershell
winget uninstall Microsoft.Winget.Source_8wekyb3d8bbwe
winget source reset --force
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

- [Snappy Driver Installer Origin](https://www.snappy-driver-installer.org/) - A portable tool to install and update device drivers
  > #### Note: DO NOT USE **'Snappy Driver Installer'**, it is known for being malware, only **'Snappy Driver Installer Origin'** -> [Reddit Thread](https://www.reddit.com/r/software/comments/ui3orx/snappy_driver_installer_vs_origin/)
- [Tron](https://github.com/bmrf/tron) - An automated PC cleanup script **(RECOMMENDED)**
- [Kasperky Rescue Disk](https://www.kaspersky.co.in/downloads/free-rescue-disk)
- [Kasperky Virus Removal Tool](https://www.kaspersky.co.in/downloads/free-virus-removal-tool)
- [Driver Store Explorer](https://github.com/lostindark/DriverStoreExplorer) - A portable tool to perform operations such as list/add/install/delete third-party driver packages and also export them use them after installing new Windows.

## Some of the recommended software

- [Shell](https://nilesoft.org/) - Powerful context menu manager for Windows File Explorer
- [ImageGlass](https://imageglass.org) - An open source, free, lightweight, versatile and ad-free image viewer.
- [7zip](https://www.7-zip.org/) - An opensource software for file archives alternative to Winrar.
- [qbittorrent](https://www.qbittorrent.org/download) - An opensource and reliable P2P BitTorrent client in C++ / Qt that uses libtorrent (sometimes called libtorrent-rasterbar) by Arvid Norberg
- [f.lux](https://justgetflux.com/) - Alternative to Windows nightlight with various options/features.
- [ShareX](https://getsharex.com/) - Alternative to windows Snipping tools for taking screenshots, record screen, pick colors,etc.
- [JDownloader](https://jdownloader.org/) - A free and open source download manager
- [Joplin](https://joplinapp.org/) - An open source note-taking app to capture thoughts and securely access them from any device.
- [Notesnook](https://notesnook.com/) - An open source, end-to-end encrypted, and private note taking app with freedom, no spying, no tracking.
- [MusicBee](https://getmusicbee.com/) - A music manager and player that makes it easy to manage, find, and play music files on your computer.
- [Bitwarden](https://bitwarden.com/) - A cross platform opensource password manager.
- [Bulk Crap Uninstaller](https://www.bcuninstaller.com/) - Bulk Crap Uninstaller (i.e. BCUninstaller or BCU) is a free bulk program uninstaller with advanced automation.
- [Revo Uninstaller](https://www.revouninstaller.com/) - Uninstall unwanted programs and their leftovers, quickly and easily!
- [Bleach Bit](https://www.bleachbit.org/) - A free and open-source disk space cleaner, privacy manager, and computer system optimizer.
- [K-Lite Codec](https://codecguide.com/) - An opensource codec application with supports many video and audio formats.
- [Kdenlive](https://kdenlive.org/en/) - A free and open source video editor.
