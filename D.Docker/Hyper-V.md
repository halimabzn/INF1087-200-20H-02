

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


PowerShell uses `$()` to evaluate sub-expressions

https://stackoverflow.com/questions/434038/whats-the-cmd-powershell-equivalent-of-back-tick-on-bash

```
PS >  docker rm $(docker container ls --all -q)
```
