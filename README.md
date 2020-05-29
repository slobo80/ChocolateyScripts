ChocolateyScripts
=================

Chocolatey scripts for installing, updating, and performing other application operations.

Fresh machine install requires:  

1. Open powershell
1. Enable powershell scripts to execute

    ```powershell
    Set-ExecutionPolicy -ExecutionPolicy Bypass`
    ```

1. Install Chocolatey

    ```powershell
    iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))
    ```

1. Clone the repo

    ```powershell
    git clone https://github.com/slobo80/ChocolateyScripts.git
    ```

1. Rename `packages-home.config` OR `packages-work.config` to `packages.config`. They contain the list of apps to install
1. Disable Chocolatey warning

    ```powershell
    choco feature enable -n=allowGlobalConfirmation
    ```

1. Install apps

    ```powershell
    install.ps1
    ```
