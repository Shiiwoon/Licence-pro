# Stockage - Haute-Dispo
# Sauvegarde Avec Déduplication

> config: Debian 


>    ### Objectif: 
- Mise en place de disques en RAID ( serveur de sauvegardes, partiel ) 
- Haute disponibilité avec 2 serveur Debian utilisant GlusterFS
        - Chaque serveur sera un miroir de l'autre et les fichier seront répliqués automatiquement entre eux.

#### Mise en place de disques en RAID ( Serveur de sauvegarde, partiel )
>****Information**** 
Avec 3 disques de 1 go
Type de RAID : RAID1

        # apt-get i nstall mdadm

> Création du RAID1 entre le 2 disques
        
        # mdadm --create /dev/md0 --level=1 --raid-devices=2 /dev/sdb /dev/sdc
        
> Vérification 
        
        # mdadm -D /dev/md0
        
> Ajout du SPARE ( remplacement )(le 3eme disque)

        # mdadm --manage /dev/md0 --add /dev/sdd
        
> Revérification 
    
        # mdadm -D /dev/md0
        
        
> 