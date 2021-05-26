# Sauvegardes avancées

Les différents types de sauvegarde avancée sont :

{% tabs %}
{% tab title="Hyper-V" %}
Pour effectuer une sauvegarde de machines virtuelles Hyper-V : 

* Installer les agents sur les machines hôtes et dans les machines virtuelles
* Sauvegarde volume du serveur Hyper-V
* Sauvegarde volume avec agents dans les machines virtuelles
{% endtab %}

{% tab title="SQL Server" %}
Pour effectuer une sauvegarde de bases SQL Server : 

* Installer les agents sur les machines hôtes
* Sélectionner les fichiers MDF/NDF et les journaux. Par défaut ceux-ci se trouvent dans le même répertoire.
* Associer une seule base par job de sauvegarde.
{% endtab %}

{% tab title="Microsoft Exchange" %}
Pour effectuer une sauvegarde en de base Microsoft Exchange : 

* Installer les agents sur les machines hôtes
* Utiliser uniquement le mode BANQUE.
* Sélectionner les fichiers EDB et les journaux. Par défaut ceux-ci se trouvent dans le même répertoire.
*  Associer une seule base par job de sauvegarde.
{% endtab %}

{% tab title="VMware ESX" %}
Pour effectuer une sauvegarde de machines virtuelles VMware ESXi : 

* Assurez vous que la version de VMware ESXi soit à minima en 5.5
* L'agent n'est pas nécessaire dans les machines virtuelles
* Si la machine virtuelle est compatible avec l'option Changed Block Tracking \(CBT\) le connecteur pourra effectuer une sauvegarde incrémentale, dans le cas contraire il s'agira d'une sauvegarde différentielle
* Le [connecteur](https://docs.yoobackup.fr/~/edit/drafts/-LZZqqmegTeaDH7RMDwR/installation/installation-des-agents-de-sauvegarde/configuration-connecteur-vmware) est à paramétrer directement dans l'interface, seuls l'IP, le login et le mot de passe du vSphere \(ou vCenter\) sont nécessaires pour configurer l'intégration du [connecteur](https://docs.yoobackup.fr/~/edit/drafts/-LZZqqmegTeaDH7RMDwR/installation/installation-des-agents-de-sauvegarde/configuration-connecteur-vmware)
*  Associer une seule machine virtuelle par job de sauvegarde.
{% endtab %}
{% endtabs %}

