# Installation d'une appliance Classic

L'installation d'une appliance Classic est simple mais doit être effectuée correctement pour assurer son bon fonctionnement.

## Vue d'ensemble

### Classic box

![](../../.gitbook/assets/image%20%281%29.png)

### Platine connectiques

![](../../.gitbook/assets/image%20%2814%29.png)

## Contenu du carton

* Une appliance Classic
* Un cordon d'alimentation \(ou une alimentation externe en fonction du modèle, cf. [Spécifications techniques](../../specifications-techniques.md#appliances-allroad)\)
* Un cable RJ45
* Un onduleur et un câble USB spécifique
* OneKey Restore

## Raccordement électrique

Nous pouvons maintenant procéder au raccordement électrique de la solution:

1. Raccorder la box à l'onduleur \(fourni avec la box en fonction de l'offre choisie\).
2. Raccorder le câble USB de l'onduleur à n'importe quel port USB de l'appliance
3. Brancher l'onduleur au réseau électrique du client

## Raccordement réseau

Toutes les solutions possèdent deux ports réseau pouvant être utilisés pour associer l'appliance à deux réseaux physiques présents au sein de l'installation.

Le port par défaut est indiqué par un autocollant LAN si ce n'est pas le cas, il s'agit du port le plus proche du port d'alimentation.

Une fois l'appliance raccordée physiquement au réseau du client, il va falloir la rendre accessible. Pour cela, 3 solutions :

1. S'il y a un DHCP et la propagation des noms d'hôtes, la machine sera disponible sur le nom d'hôte "wooxo-desktop"
2. Vous avez la possibilité d'utiliser WTool qui est un utilitaire créé par Wooxo \([téléchargeable ici](https://wooxo.fr/WTool)\) 
3. Directement depuis l'appliance à l'aide d'un clavier/écran et du compte de maintenance \(identifiant : config / mot de passe: config\)

![](../../.gitbook/assets/image%20%2810%29.png)

