

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
