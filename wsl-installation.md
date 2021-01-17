* Follow [this guideline](https://docs.microsoft.com/en-us/windows/wsl/) to install WSL on Windows.

```
dism.exe /online /enable-feature /featurename:Microsoft-Windows-Subsystem-Linux /all /norestart
dism.exe /online /enable-feature /featurename:VirtualMachinePlatform /all /norestart
wsl --set-default-version 2
```

* Use Windows Terminal to connect to the designated Linux distribution.
* Follow [this instruction](https://docs.microsoft.com/en-us/powershell/scripting/install/installing-powershell-core-on-linux) to install PowerShell Core on the Linux distribution.
* Open ~/.bashrc file with nano ~/.bashrc and add `pwsh` to start PowerShell Core by default when opening the terminal.
