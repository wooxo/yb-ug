# Sauvegardes avancées

Les différents types de sauvegarde avancée sont :

{% tabs %}
{% tab title="Hyper-V" %}
Pour effectuer une sauvegarde de machine virtuelles Hyper-V : 

* Installer les agents sur les machines hôtes
* Sélectionner les fichiers VHD/A VHD
* Associer une seule machine virtuelle par job de sauvegarde.
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
Pour effectuer une sauvegarde en utilisant VMware ESX : 

* Assurez vous que la version VMware ESX soit compatible avec une version 4.1 et supérieures
* Si la machine virtuelle contient l'option Changed Block Tacking \(CBT\) le connecteur pourra effectuer une sauvegarde incrémentale, dans le cas contraire il s'agira d'une sauvegarde différentielle
* Le [connecteur](https://docs.yoobackup.fr/~/edit/drafts/-LZZqqmegTeaDH7RMDwR/installation/installation-des-agents-de-sauvegarde/configuration-connecteur-vmware) est à paramétrer directement dans l'interface, seuls l'IP, le login et le mot de passe du vSphere \(ou vCenter\) sont nécessaires pour configurer l'intégration du [connecteur](https://docs.yoobackup.fr/~/edit/drafts/-LZZqqmegTeaDH7RMDwR/installation/installation-des-agents-de-sauvegarde/configuration-connecteur-vmware)
*  Associer une seule machine virtuelle par job de sauvegarde.
{% endtab %}
{% endtabs %}

