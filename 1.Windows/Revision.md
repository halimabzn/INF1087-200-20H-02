# Revision Test Windows


## :one: Installation Proliant

* Installation sur Proliant GX

  :pushpin: Création de Clé USB:
   
    - Télécharger ISO sur Azure Education
    
    Logicel de boot de clé USB ? (Rufus, UnetBooting)
    
    Option pour booter la clé : 
      
    * Master Boot Record [MBR](https://github.com/CollegeBoreal/Tutoriels/tree/master/7.Microsoft/servers/ISO) 

    * GUID Partition Table (GPT)

    * Preboot Execution Environment (PXE)
    
    [:bulb: GPT vs MBR](https://www.howtogeek.com/193669/whats-the-difference-between-gpt-and-mbr-when-partitioning-a-drive)

   * Trouble Shoot quand boot unsuccessful

     [RedScreenOfDeath](https://github.com/CollegeBoreal/Laboratoires/blob/master/3202/proliant/TroubleShoot.md#pushpin-red-screen-of-death) 
     
  :pushpin: Boot
  
     * Basic Input Output System (BIOS)
     
     * Unified Extensible Firmware Interface (UEFI)
     
     [:bulb: BIOS vs UEFI](https://www.howtogeek.com/56958/htg-explains-how-uefi-will-replace-the-bios/)
       
    ISO Choisi ou suggéré
    
    - Windows Server 2019 - [Standard, Essential, Datacenter]
    
    - Windows `Hyper-V` Server 2019
    
   :pushpin: Disques [RAID](https://github.com/CollegeBoreal/Laboratoires/tree/master/3202/proliant/RAID)
   
    - Booter sur RAID Setup Utility `F8`
    
    - RAID :five: exigences
    
      formatter `3` disques minimum
      
    - Créer des disques logiques
    
      soit 3 disques a 146Gb donne 438Gb au final en RAID5 273Gb approxivement 62% de capacité d'utilisation
      
      soit 40% utilisé pour redondance pour `hot swap`

## :two: Installation de Windows 

https://github.com/CollegeBoreal/Tutoriels/tree/master/7.Microsoft/servers/core
   
   
      * Passe d'un écran à un autre
      
      - Configuration Language, Clavier et Format Temps Et Devises
      
      - Accepter la license 
      
      - choisir Upgrade ou Custom
      
      - Installation sur le disque (choix de formatter les partitions) - :warning: Boot disk on line
      
      - Déroulement de l'installation (puis reboot)
      
      - Demande le changement de mot de passe de l'administrateur - `Administrator`
      
      - Mot de passe suit une `Politique de sécurité` - 
      
          Règle - Une Majuscule, Une Minuscule, un chiffre, un symbole ($,!) et une taille (6)
          
      - Fenetres de configurations: 
      
        * Script de configuration s'appelle `Sconfig.cmd`
        
        * $HOME directory de l'Administrateur : c:\Users\Administrator
        
        
      - Script Configuration en réseau: (RDP - Remote Desktop)
      
          * Sélection de l'adaptateur réseau (il faut le brancher)
      
          * Changer les nom de la machine (Optionnel)
          
          * Changer la configuration du réseau (IP Statique/Masque/GW/DNS)
          
          * Enable RDP
          
          (Reboot)


### :o: Remote Desktop

https://github.com/CollegeBoreal/Tutoriels/tree/master/7.Microsoft/servers/core#utilisation-a-distance

 * Accès coté client
 
    RDP:
    
    * Adresse IP
    
    * Nom
    
    * Mot de passe
          
          
          
      
      
      
      
      
      
      
   
     
    
    
   


