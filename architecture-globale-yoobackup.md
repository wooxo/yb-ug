# Architecture et fonctionnement YooBackup

## Généralités

![](.gitbook/assets/image%20%2813%29.png)

### Fonctionnement global

Sur chaque élément à sauvegarder, il est nécessaire d'installer un agent YooBackup qui réalisera une sauvegarde cryptée et compressée \(fichiers ou volume\) dès l'origine vers un stockage principal, une appliance dans la plupart des cas.

Cette sauvegarde pourra être externalisée vers un stockage secondaire : cloud Wooxo ou une deuxième appliance.

Dans le cas où un agent n'arrive pas à joindre son stockage principal pour une raison quelconque \(indisponibilité, panne, agent en itinérance\), il ira, s'il est configuré en réplication externalisée, contacter directement le stockage secondaire vers lequel il sauvegardera. Lorsque le stockage principal sera de nouveau joignable, les données redescendront automatiquement. C'est ce que l'on appelle le Plan de Continuité de Sauvegarde \(PCS\).

### Un système de sauvegarde incrémentale bloc illimité

YooBackup utilise une technologie permettant de fournir un système de sauvegarde incrémentale bloc illimité.

À chaque sauvegarde le système va identifier les éléments ayant évolué depuis l'opération précédente. À partir de là, objet par objet il va identifier les blocs ayant évolué et ne sauvegarder ainsi que l'incrément.

Au moment de la configuration, l'utilisateur va choisir un nombre maximum de versions à conserver. Le système de sauvegarde gérera ainsi automatiquement le nombre d'incréments à conserver.  
Quand il atteindra le nombre maximum à conserver, il réalisera une opération de synthèse du premier incrément avec la première version complète pour respecter le paramétrage réalisé.

Ainsi, plus le nombre de versions à conserver est grand, plus le système sera flexible pour revenir sur des versions antérieures, mais plus l'espace de stockage nécessaire sera important.

### Encryption et sécurité

Chaque solution possède une clé de cryptage propre générée à l'activation de la solution.

Chaque agent communique avec l'appliance à travers un tunnel sécurisé.

L'ensemble des données sont cryptées à la source à l'aide de la clé propre à l'appliance.

Cette clé et l'ensemble des configurations propres à l'appliance sont sauvegardées de manière régulière et sécurisée vers la seconde appliance ou l'infrastructure Wooxo pour permettre le fonctionnement de la continuité de sauvegarde et également permettre une reprise en cas de sinistre majeur sur l'appliance.

L'ensemble des données stockées physiquement sur l'appliance sont cryptées, compressés et ventilées via le système de gestion des versions, et donc inutilisables en l'état en cas d'extraction ou de manipulation physique sur l'appliance.

## Composants techniques

![](.gitbook/assets/image%20%2822%29.png)

