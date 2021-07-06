# Advanced Backup

The different types of advanced backups are:

{% tabs %}
{% tab title="Hyper-V" %}
To perform a backup of Hyper-V virtual machines: 

* Install agents on host machines and in virtual machines
* Hyper-V server volume backup
* Volume backup with agents in virtual machines
{% endtab %}

{% tab title="SQL Server" %}
To perform a backup of a SQL Server : 

* Install agents on host machines
* Select MDF/NDF files and logs. By default they are in the same directory.
* Associate a single database with a backup job.
{% endtab %}

{% tab title="Microsoft Exchange" %}
To perform a backup of a Microsoft Exchange :

* Install agents on host machines
* Use only BANQUE mode.
* Select EDB files and logs. By default they are in the same directory.
*  Associate a single database with a backup job.
{% endtab %}

{% tab title="VMware ESX" %}
To perform a backup of VMware ESXi virtual machines :

*  Make sure that the VMware ESXi version is at least 5.5
* The agent is not required in virtual machines
* If the virtual machine is compatible with the Changed Block Tracking \(CBT\) option the connector will be able to perform an incremental backup, otherwise it will be a differential backup
* The [connector](https://docs.yoobackup.fr/~/edit/drafts/-LWjtVvwDwbXk_mJzQSr/v/english/installation/installation-des-agents-de-sauvegarde/configuration-connecteur-vmware) needs to be configured in the interface, only the vSphere \(or vCenter\) IP, login, and password are needed to configure the connector integration.
*  Associate a single virtual machine with a backup job.
{% endtab %}
{% endtabs %}

