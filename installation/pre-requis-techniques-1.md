# Pré-requis techniques

## Conditions de fonctionnement

Les appliances doivent être placées dans un environnement adapté au fonctionnement d'un matériel informatique :

* Ne pas exposer au soleil ou à toute flamme&#x20;
* Ne pas exposer à tout liquide quel qu'il soit
* Veiller à maintenir une température ambiante comprise entre 5 et 50 ˚C en fonctionnement.
* Raccorder l'équipement via le plug à un réseau électrique aux normes en vigueur&#x20;

En cas d'exposition à une flamme ou à tout liquide merci de vous rapprocher au plus tôt du Support Wooxo et ne pas intervenir en autonomie.

Tout fonctionnement "hors-cadre" entrainera une révocation de la garantie.

## Pré-requis réseau

### Communication appliance -> Infrastructure Wooxo/Atempo

L'appliance a besoin de communiquer avec l'infrastructure de Wooxo/Atempo pour récupérer les mises à jour, remonter les alertes et permettre le monitoring des solutions.

| Hostname         | Port(s) TCP                                                                    | Description                                              |
| ---------------- | ------------------------------------------------------------------------------ | -------------------------------------------------------- |
| api.wooxo.fr     | 443                                                                            | Monitoring matériel                                      |
| secure.wooxo.fr  | 443                                                                            | Activation des licences                                  |
| portail.wooxo.fr | 443                                                                            | Monitoring logiciel                                      |
| m0.wooxo.fr      | <p>6670 ou</p><p>80 ou</p><p>21 ou </p><p>123 ou </p><p>1720 ou</p><p>1723</p> | Prise en main maintenance (Support)                      |
| dn03.wooxo.fr    | 6670                                                                           | Brique datacenter YooBackup (alertes et externalisation) |
| repo.wooxo.fr    | <p>443 ou</p><p>80</p>                                                         | Serveur mise à jour YooBackup                            |
| packet.wooxo.fr  | <p>443 ou</p><p>80</p>                                                         | Serveur mise à jour YooBackup secondaire                 |

### Communication  appliance -> agent de sauvegarde

La communication utilise le port 6680 en TCP.

### Communication agent de sauvegarde -> appliance ou datacentre

La communication se fait sur le port 6670 en TCP et à l'installation cela nécessite le port 443 en TCP.
