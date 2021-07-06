# Configuration connecteur partage SMB/CIFS

Pour réaliser la sauvegarde d'un partage réseau Windows \(SMB/CIFS\), aucune installation d'agent n'est requise. L'agent intégré dans l'appliance sera utilsié pour effectuer la sauvegarde.

{% hint style="info" %}
Seul le protocole SMB v2 est actuellement supporté. 
{% endhint %}

A l'activation de la solution, l'agent embarqué dans l'appliance est installé, il portera le même nom d'hôte que l'appliance.

Si l'agent ne s'est pas déployé, vous pouvez vous rendre dans l'administration et forcer son installation.

Une fois l'agent disponible, il suffit de le sélectionner:

![](../../.gitbook/assets/image%20%2834%29.png)

De se rendre dans l'onglet "Partages distant" sur la droite :

![](../../.gitbook/assets/image%20%2817%29.png)

Et de créer un nouveau partage

![](../../.gitbook/assets/image%20%2810%29.png)

Il faut préciser un nom du partage permettant de l'identifier facilement par la suite, l'adresse réseau, le point de montage ainsi que les identifiants de montage \(ne pas renseigner le domaine, il sera automatiquement détecté\). 

