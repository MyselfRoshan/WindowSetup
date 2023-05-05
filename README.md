Install Window without any debloat
Download the Windows.iso and create installation media.
Step 1 : Click the links below to download official Windows ISO :

Windows 10
Windows 11
Step 2 : Create bootable USB drive using program metioned below :

Ventoy (Recommended)
Etcher (Beginner Friendly)
Rufus
Some famous debloating scripts (Recommended)
irm -useb https://christitus.com/win | iex
irm -useb https://git.io/debloat | iex
Install Enterprise LTSC version of windows without any bloat
Install winget, choco, scoop packet manager (Optional)
Note: Use Ctrl+V within Powershell(with Administrator) to run all code at once

Step 1 : To install winget without Microsoft Store

Set-PSRepository -Name 'PSGallery' -InstallationPolicy Trusted
Install-Script -Name winget-install -Force
winget-install.ps1
Step 2 : To install choco

Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://community.chocolatey.org/install.ps1'))
Step 3 : To install scoop

Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
irm get.scoop.sh | iex
Some of the system utility tools
Tron - An automated PC cleanup script (RECOMMENDED)
Kasperky Rescue Disk
Kasperky Virus Removal Tool
