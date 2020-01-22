# Serveurs Windows


|:hash:| :id:      | Utilisateur à remplacer | RDP              | Docker Engine    | 
|------|-----------|-------------------------|------------------|------------------|
| 01   | 300104524 | Brice@10.13.237.19      |:x:               |:x:               |
| 02   | 300104541 | Brice@10.13.237.:bangbang: |:x:            |:x:               |
| 03   | 300106918 | Brice@10.13.237.18      |:x:               |:x:               |
| 04   | 300107361 | Brice@10.13.237.99      |:heavy_check_mark:|:x:               |
| 05   | 300108234 | Brice@10.13.237.55      |:x:               |:x:               |
| 06   | 300110500 | Brice@10.13.237.75      |:x:               |:x:               |
| 07   | 300110529 | Brice@10.13.237.80      |:x:               |:x:               |
| 08   | 300111671 | Brice@10.13.237.63      |:x:               |:x:               |
| 09   | 300111766 | Brice@10.13.237.66      |:x:               |:x:               |
| 10   | 300112017 | Brice@10.13.237.60      |:x:               |:x:               |
| 11   | 300112917 | Brice@10.13.237.79      |:x:               |:x:               |
| 12   | 300113775 | Brice@10.13.237.77      |:x:               |:x:               |


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
