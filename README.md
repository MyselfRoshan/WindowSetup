# Install Window without any debloat
## Download the Windows.iso file
`Step 1 :` Click [here](https://www.microsoft.com/en-us/software-download/windows10/) to visit the microsoft official website.

## Some famous debloating scripts
```powershell
irm -useb https://christitus.com/win | iex
```
```powershell
irm -useb https://git.io/debloat | iex
```
## Activate Windows
```powershell
irm https://massgrave.dev/get | iex
```
## Install Enterprise LTSC version of window without any bloat
## Install winget, choco, scoop packet manager
*`Note: Use Ctrl+V within Powershell(with Administrator) to run all code at once`*

`Step 1 :` To install scoop
```powershell
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
irm get.scoop.sh | iex
```
`Step 2 :` To install winget without Microsoft Store
```powershell
Set-PSRepository -Name 'PSGallery' -InstallationPolicy Trusted
Install-Script -Name winget-install -Force
winget-install.ps1
```
