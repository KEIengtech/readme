- 관리자모드로 파워쉘 열기
- 초콜러티 설치
~~~
Set-ExecutionPolicy Bypass -Scope Process -Force; `
[System.Net.ServicePointManager]::SecurityProtocol = `
[System.Net.ServicePointManager]::SecurityProtocol -bor 3072; `
iex ((New-Object System.Net.WebClient).DownloadString('https://community.chocolatey.org/install.ps1'))
~~~
~~~
PS C:\Windows\system32> Set-ExecutionPolicy Bypass -Scope Process -Force; `
>> [System.Net.ServicePointManager]::SecurityProtocol = `
>> [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; `
>> iex ((New-Object System.Net.WebClient).DownloadString('https://community.chocolatey.org/install.ps1'))
Forcing web requests to allow TLS v1.2 (Required for requests to Chocolatey.org)
Getting latest version of the Chocolatey package for download.
Not using proxy.
Getting Chocolatey from https://community.chocolatey.org/api/v2/package/chocolatey/2.6.0.
Downloading https://community.chocolatey.org/api/v2/package/chocolatey/2.6.0 to C:\Users\번개곰돌\AppData\Local\Temp\chocolatey\chocoInstall\chocolatey.zip
Not using proxy.
Extracting C:\Users\번개곰돌\AppData\Local\Temp\chocolatey\chocoInstall\chocolatey.zip to C:\Users\번개곰돌\AppData\Local\Temp\chocolatey\chocoInstall
Installing Chocolatey on the local machine
Creating ChocolateyInstall as an environment variable (targeting 'Machine')
  Setting ChocolateyInstall to 'C:\ProgramData\chocolatey'
WARNING: It's very likely you will need to close and reopen your shell
  before you can use choco.
Restricting write permissions to Administrators
We are setting up the Chocolatey package repository.
The packages themselves go to 'C:\ProgramData\chocolatey\lib'
  (i.e. C:\ProgramData\chocolatey\lib\yourPackageName).
A shim file for the command line goes to 'C:\ProgramData\chocolatey\bin'
  and points to an executable in 'C:\ProgramData\chocolatey\lib\yourPackageName'.

Creating Chocolatey CLI folders if they do not already exist.

chocolatey.nupkg file not installed in lib.
 Attempting to locate it from bootstrapper.
PATH environment variable does not have C:\ProgramData\chocolatey\bin in it. Adding...
경고: Not setting tab completion: Profile file does not exist at
'C:\Users\번개곰돌\Documents\WindowsPowerShell\Microsoft.PowerShell_profile.ps1'.
Chocolatey CLI (choco.exe) is now ready.
You can call choco from anywhere, command line or PowerShell by typing choco.
Run choco /? for a list of functions.
You may need to shut down and restart PowerShell and/or consoles
 first prior to using choco.
Ensuring Chocolatey commands are on the path
Ensuring chocolatey.nupkg is in the lib folder
PS C:\Windows\system32> choco install nodejs
>> choco install git
Chocolatey v2.6.0
Installing the following packages:
nodejs
By installing, you accept licenses for the packages.
Downloading package from source 'https://community.chocolatey.org/api/v2/'
Progress: Downloading nodejs.install 25.8.0... 100%

nodejs.install v25.8.0 [Approved]
nodejs.install package files install completed. Performing other installation steps.
The package nodejs.install wants to run 'chocolateyInstall.ps1'.
Note: If you don't run this script, the installation will fail.
Note: To confirm automatically next time, use '-y' or consider:
choco feature enable -n allowGlobalConfirmation
Do you want to run the script?([Y]es/[A]ll scripts/[N]o/[P]rint):

Timeout or your choice of '' is not a valid selection.
You must select an answer
Do you want to run the script?([Y]es/[A]ll scripts/[N]o/[P]rint): Y

Installing 64-bit nodejs.install...
nodejs.install has been installed.
  nodejs.install may be able to be automatically uninstalled.
Environment Vars (like PATH) have changed. Close/reopen your shell to
 see the changes (or in powershell/cmd.exe just type `refreshenv`).
 The install of nodejs.install was successful.
  Software installed as 'msi', install location is likely default.
Downloading package from source 'https://community.chocolatey.org/api/v2/'
Progress: Downloading nodejs 25.8.0... 100%

nodejs v25.8.0 [Approved]
nodejs package files install completed. Performing other installation steps.
 The install of nodejs was successful.
  Deployed to 'C:\ProgramData\chocolatey\lib\nodejs'

Chocolatey installed 2/2 packages.
 See the log for details (C:\ProgramData\chocolatey\logs\chocolatey.log).
Chocolatey v2.6.0
Installing the following packages:
git
By installing, you accept licenses for the packages.
Downloading package from source 'https://community.chocolatey.org/api/v2/'
Progress: Downloading chocolatey-compatibility.extension 1.0.0... 100%

chocolatey-compatibility.extension v1.0.0 [Approved]
chocolatey-compatibility.extension package files install completed. Performing other installation steps.
 Installed/updated chocolatey-compatibility extensions.
 The install of chocolatey-compatibility.extension was successful.
  Deployed to 'C:\ProgramData\chocolatey\extensions\chocolatey-compatibility'
Downloading package from source 'https://community.chocolatey.org/api/v2/'
Progress: Downloading chocolatey-core.extension 1.4.0... 100%

chocolatey-core.extension v1.4.0 [Approved]
chocolatey-core.extension package files install completed. Performing other installation steps.
 Installed/updated chocolatey-core extensions.
 The install of chocolatey-core.extension was successful.
  Deployed to 'C:\ProgramData\chocolatey\extensions\chocolatey-core'
Downloading package from source 'https://community.chocolatey.org/api/v2/'
Progress: Downloading git.install 2.53.0... 100%

git.install v2.53.0 [Approved]
git.install package files install completed. Performing other installation steps.
The package git.install wants to run 'chocolateyInstall.ps1'.
Note: If you don't run this script, the installation will fail.
Note: To confirm automatically next time, use '-y' or consider:
choco feature enable -n allowGlobalConfirmation
Do you want to run the script?([Y]es/[A]ll scripts/[N]o/[P]rint): Y

Using Git LFS
Installing 64-bit git.install...
git.install has been installed.
git.install installed to 'C:\Program Files\Git'
  git.install can be automatically uninstalled.
Environment Vars (like PATH) have changed. Close/reopen your shell to
 see the changes (or in powershell/cmd.exe just type `refreshenv`).
 The install of git.install was successful.
  Deployed to 'C:\Program Files\Git\'
Downloading package from source 'https://community.chocolatey.org/api/v2/'
Progress: Downloading git 2.53.0... 100%

git v2.53.0 [Approved]
git package files install completed. Performing other installation steps.
 The install of git was successful.
  Deployed to 'C:\ProgramData\chocolatey\lib\git'

Chocolatey installed 4/4 packages.
 See the log for details (C:\ProgramData\chocolatey\logs\chocolatey.log).
PS C:\Windows\system32> choco install pyenv-win
Chocolatey v2.6.0
Installing the following packages:
pyenv-win
By installing, you accept licenses for the packages.
Downloading package from source 'https://community.chocolatey.org/api/v2/'
Progress: Downloading pyenv-win 3.1.1... 100%

pyenv-win v3.1.1 [Approved]
pyenv-win package files install completed. Performing other installation steps.
The package pyenv-win wants to run 'chocolateyInstall.ps1'.
Note: If you don't run this script, the installation will fail.
Note: To confirm automatically next time, use '-y' or consider:
choco feature enable -n allowGlobalConfirmation
Do you want to run the script?([Y]es/[A]ll scripts/[N]o/[P]rint): Y

Attempt to use original download file name failed for 'C:\ProgramData\chocolatey\lib\pyenv-win\tools/pyenv-win.zip'.
Copying pyenv-win
  from 'C:\ProgramData\chocolatey\lib\pyenv-win\tools/pyenv-win.zip'
Hashes match.
Extracting C:\Users\번개곰돌\AppData\Local\Temp\chocolatey\pyenv-win\3.1.1\pyenv-winInstall.zip to C:\Users\번개곰돌\.pyenv\...
C:\Users\번개곰돌\.pyenv\
PATH environment variable does not have %USERPROFILE%\.pyenv\pyenv-win\bin in it. Adding...
PATH environment variable does not have %USERPROFILE%\.pyenv\pyenv-win\shims in it. Adding...
Environment Vars (like PATH) have changed. Close/reopen your shell to
 see the changes (or in powershell/cmd.exe just type `refreshenv`).
 The install of pyenv-win was successful.
  Deployed to 'C:\Users\번개곰돌\.pyenv\'

Chocolatey installed 1/1 packages.
 See the log for details (C:\ProgramData\chocolatey\logs\chocolatey.log).
PS C:\Windows\system32>
~~~
