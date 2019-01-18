# Guide de compatibilités

## Sauvegarde fichiers

![](../../.gitbook/assets/image%20%288%29.png)

* Windows Seven jusqu'à Windows 10
* Windows Server 2008 R2 jusqu'à Windows Server 2016

![](../../.gitbook/assets/image%20%282%29.png)

* MacOs 10.12 jusqu'à macOS 10.14

![](../../.gitbook/assets/image%20%2818%29.png)

* Debian 7 jusqu'à Debian 9
* Ubuntu 10 jusqu'à Ubuntu 18
* RedHat 6 jusqu'à RedHat 7 
* Fedora 22 jusqu'à Fedora 28 
* CentOs 6 jusqu'à CentOS 7

## Sauvegarde volume \(BMR\)

![](../../.gitbook/assets/image%20%288%29.png)

* Windows Seven jusqu'à Windows 10
* Windows Server 2008 R2 jusqu'à Windows Server 2016

## Sauvegarde hyperviseur

![](../../.gitbook/assets/image%20%288%29.png)

* Hyper-V: 
  * Windows Server 2008 R2 / Windows Server 2012 / Windows Server 2012 R2
  * Pas de support des clusters

![](../../.gitbook/assets/image%20%2826%29.png)

* VMware vSphere
  * Version 4.1 à 6.7
  * Support de CBT 
  * Support de vCenter

## Sauvegarde applicative

![](../../.gitbook/assets/image%20%288%29.png)

* Microsoft SLQ Server
  * Base complète en mode fichier à chaud
* Microsoft Exchange
  * Base complète en mode fichier à chaud
* Microsoft SharePoint
  * Instance complète en mode fichier à chaud
  * Nécessite la déclaration du Writer VSS au préalable
* Oracle Database
  * Version 11 et supérieur
  * Nécessite de valider la déclaration du Writer VSS au préalable

 



