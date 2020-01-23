# Revision Test Windows


:one: Installation

* Installation sur Proliant GX

  :pushpin: Création de Clé USB:
   
    - Télécharger ISO sur Azure Education
    
    Logicel de boot de clé USB ? (Rufus, UnetBooting)
    
    Option pour booter la clé : 
      
      * Master Boot Record (MBR) 
      
      * GUID Partition Table (GPT)
      
      * Preboot Execution Environment (PXE)

   * Trouble Shoot quand boot unsuccessfull 

     [RedScreenOfDeath](https://github.com/CollegeBoreal/Laboratoires/blob/master/3202/proliant/TroubleShoot.md#pushpin-red-screen-of-death) 
       
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
      
    
    
   


