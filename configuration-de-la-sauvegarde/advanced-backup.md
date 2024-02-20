# Advanced Backup

The different types of advanced backups are:

{% tabs %}
{% tab title="Hyper-V" %}
To perform a backup of Hyper-V virtual machines: 

* Install agents on host machines
* Select VHD/A VHD files
* Associate a single virtual machine with a backup job.
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
To perform a backup using VMware ESX: 

* Make sure the VMware ESX version is compatible with version 4.1 and above. 
* If the Virtual machine has the option Changed Block Tacking \(CBT\), YooBackup will perform an incremental backup, otherwise it will be a differential backup.
* The [connector](https://docs.yoobackup.fr/~/edit/drafts/-LWjtVvwDwbXk_mJzQSr/v/english/installation/installation-des-agents-de-sauvegarde/configuration-connecteur-vmware) needs to be configured in the interface, only the vSphere \(or vCenter\) IP, login, and password are needed to configure the connector integration.
*  Associate a single virtual machine with a backup job.
{% endtab %}
{% endtabs %}
