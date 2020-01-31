

```
PS > Get-WindowsFeature *Hyper*

Display Name                                            Name                       Install State
------------                                            ----                       -------------
[X] Hyper-V                                             Hyper-V                        Installed
        [ ] Hyper-V Management Tools                    RSAT-Hyper-V-Tools             Available
            [ ] Hyper-V Module for Windows PowerShell   Hyper-V-PowerShell             Available
```


```
PS > Get-VMSwitch  *

Name                   SwitchType NetAdapterInterfaceDescription
----                   ---------- ------------------------------
Primary Virtual Switch External   QLogic BCM5709C Gigabit Ethernet (NDIS VBD Client) #4
nat                    Internal
```

Create a new Disk

```
PS >  New-VHD -Path .\VMs\Win10.vhdx -Fixed -SizeBytes 1GB
```
Create the new VM

```
PS >   New-VM -Name Win10VM -MemoryStartupBytes 4GB -BootDevice VHD -VHDPath .\VMs\Win10.vhdx -Path .\VMData -Generation 2 -Switch "Primary Virtual Switch"
```

REMOVE VM

```
PS >  Remove-VM Win10VM
```

Remove all Data


```
PS > Get-ChildItem -Path .\VMData\ -Include *.* -Recurse | foreach { $_.Delete()}
```



https://docs.microsoft.com/en-us/powershell/module/hyper-v/new-vhd?view=win10-ps


PowerShell uses `$()` to evaluate sub-expressions

https://stackoverflow.com/questions/434038/whats-the-cmd-powershell-equivalent-of-back-tick-on-bash

```
PS >  docker rm $(docker container ls --all -q)
```
