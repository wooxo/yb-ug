# Configuration connecteur montages SAMBA

 Pour réaliser la sauvegarde de montage SAMBA, il n'est pas nécessaire de déployer un agent sur les éléments à sauvegarder.

A l'activation de la solution, l'agent embarqué dans l'appliance est installé, il portera le même nom d'hôte que l'appliance.

Si l'agent ne s'est pas déployé, vous pouvez vous rendre dans l'administration et forcer son installation.

Une fois l'agent disponible, il suffit de le sélectionner:

![](../../.gitbook/assets/image%20%2830%29.png)

De se rendre dans l'onglet "Partages distant" sur la droite:

![](../../.gitbook/assets/image%20%2816%29.png)

Et de créer un nouveau partage

![](../../.gitbook/assets/image%20%289%29.png)

Il faut préciser un nom du partage permettant de l'identifier facilement par la suite, l'adresse réseau, le point de montage ainsi que les identifiants de montage \(ne pas renseigner le domaine, il sera automatiquement détecté\). 

