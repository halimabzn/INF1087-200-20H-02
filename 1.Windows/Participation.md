# Serveurs Windows


|:hash:| :id:      | Utilisateur à remplacer | RDP                 | Docker Engine (Optionnel)    | 
|------|-----------|-------------------------|-----------------------------------------|-------------------|
| 01   | 300104524 | Brice@10.13.237.19      |:heavy_check_mark: - Hyper-V |:x:                |
| 02   | 300104541 | Brice@10.13.237.41      |:heavy_check_mark: - Hyper-V |:x:                |
| 03   | 300106918 | Brice@10.13.237.18      |:heavy_check_mark: - Datacenter :keyboard: :key: | :heavy_check_mark: |
| 04   | 300107361 | Brice@10.13.237.99      |:heavy_check_mark: - Hyper-V             |:x:               |
| 05   | 300108234 | Brice@10.13.237.55      |:heavy_check_mark: - Hyper-V             |:x:                |
| 06   | 300110500 | Brice@10.13.237.75      |:heavy_check_mark: - Hyper-V             |:x:                |
| 07   | 300110529 | Brice@10.13.237.80      |:heavy_check_mark: - Datacenter :desktop_computer: :key: |:x:                |
| 08   | 300111671 | Brice@10.13.237.63      |:heavy_check_mark: - Datacenter :keyboard: :key: |:heavy_check_mark:                |
| 09   | 300111766 | Brice@10.13.237.66      |:heavy_check_mark: - Datacenter :keyboard: :key: |:x:                |
| 10   | 300112017 | Brice@10.13.237.60      |:heavy_check_mark: - Datacenter :desktop_computer: :key: |:x:               |
| 11   | 300112917 | Brice@10.13.237.79      |:x:   |:x:                |
| 12   | 300113775 | Brice@10.13.237.77      |:heavy_check_mark: - Hyper-V             |:x:               |


# Vérification Prof

Sous @PowerShell

#### :one: Entrer la commande ci-dessous, 

* Taper Enter et Donner `B0r34l$` comme mot de passe

```
PS > $Password = Read-Host -AsSecureString 
```

#### :two: Créer l'utilisateur

```
PS > New-LocalUser "Brice" -Password $Password -FullName "Brice" -Description "Prof. "
```

#### :three: Donner les droits administrateurs à l'utilisateur

```
PS > Add-LocalGroupMember -Group "Administrators" -Member "Brice"
```


# Références

https://pureinfotech.com/create-new-user-account-powershell-windows-10/
