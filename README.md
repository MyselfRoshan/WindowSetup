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

`Step 2 :` To install scoop

```powershell
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
irm get.scoop.sh | iex
```