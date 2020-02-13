# Hyper V 

## Qu'est-ce que Hyper V


## Installer le role [Hyper V](https://docs.microsoft.com/en-us/windows-server/virtualization/hyper-v/get-started/install-the-hyper-v-role-on-windows-server) sur Windows Server

```
PS> Install-WindowsFeature -Name Hyper-V -IncludeManagementTools -Restart
```


## Tester le role Hyper V et les outils de gestion `RSAT`

```
PS> Get-WindowsFeature *Hyper*

Display Name                                            Name                       Install State
------------                                            ----                       -------------
[X] Hyper-V                                             Hyper-V                        Installed
        [X] Hyper-V Management Tools                    RSAT-Hyper-V-Tools             Installed
            [X] Hyper-V Module for Windows PowerShell   Hyper-V-PowerShell             Installed
```


```
PS> Get-Module -ListAvailable *Hyper*


    Directory: C:\Windows\system32\WindowsPowerShell\v1.0\Modules


ModuleType Version    Name                                ExportedCommands
---------- -------    ----                                ----------------
Binary     2.0.0.0    Hyper-V                             {Add-VMAssignableDevice, Add-VMDvdDrive, Add-VMFibreChan...
Binary     1.1        Hyper-V                             {Add-VMDvdDrive, Add-VMFibreChannelHba, Add-VMHardDiskDr...

```

## Voir les commandes Powershell pour le role Hyper V

```
PS> Get-Command -Module Hyper-V
```
