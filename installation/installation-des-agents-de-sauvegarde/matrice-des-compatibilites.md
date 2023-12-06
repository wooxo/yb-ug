# Compatibility Guide

## Backup Files

![](<../../.gitbook/assets/image (9).png>)

* Windows 10 / 11
* Windows Server 2016 / 2019 / 2022

![](<../../.gitbook/assets/image (2).png>)

* macOs 10.15 and earlier versions

![](<../../.gitbook/assets/image (19).png>)

* Debian 9 and earlier versions
* Ubuntu 20.04 and earlier versions
* RedHat 7 and earlier versions
* Fedora 35 and earlier versions
* CentOS 7 and earlier versions

![](<../../.gitbook/assets/image (32).png>)

* DSM 6 only
* Architecture x86\_x64 & Armada370

## Volume Backup (BMR)

![](<../../.gitbook/assets/image (9).png>)

* Windows 10 / 11
* Windows Server 2016 / 2019 / 2022



## Hypervisor Backup

![](<../../.gitbook/assets/image (9).png>)

*   Hyper-V:

    * Windows Server 2016 / 2019 / 2022 (no support for clusters)



![](<../../.gitbook/assets/image (29).png>)

* VMware vSphere&#x20;
  * Version 6.5 / 6.7 / 7.0 / 8.0
  * CBT Support
  * Supports both Standalone ESXi and vCenter

## Application Backup

![](<../../.gitbook/assets/image (9).png>)

* Microsoft SQL Server
  * Full database in hot file mode
* Microsoft Exchange
  * Full database in hot file mode
* Microsoft SharePoint
  * Full instance in hot file mode
* Any other databases : backup database dump using Yoobackup

**Note :** All applications backups require a correct and working configuration of VSS writers to work properly.
