# YooBackup Architecture and Operation

## General Information

![](.gitbook/assets/image%20%2813%29.png)

### Overal Operation

On each item to backup, a YooBackup agent needs to be installed that will performed an encrypted and compressed backup \(files or volume\) from the source to a main storage, an appliance in most cases.

This backup can be outsourced to secondary storage: Wooxo Cloud or a second appliance. 

In the case where an agent cannot connect to its main storage for any reason \(unavailability, outage, agent roaming\), it will, if it is configured in outsourcing, directly contact the secondary storage to which it will be backed up. When the main storage is again reachable, the data will automatically back down. This is called the Backup Continuity Plan \(BCP\). 

### An Incremental Block backup System Unlimited 

YooBackup uses a technology to provide an incremental block backup system unlimited . 

At each backup, the system identifies the items that changes from the previous operation. From there, object by object, it identifies the blocks that change and only saves the increment.

At the configuration time, the user chooses a maximum number of versions to keep. The backup system will automatically manage the number of increments to keep.  
When it reaches the maximum numbers to keep, it will perform an operation of synthesis of the first increment with the first complete version to respect the configuration performed. 

Thus, the largest the number of versions to keep, the flexible the system will be to revert to previous versions, but more storage space will be required. 

### Encryption and security

Each solution has its own encryption key, generated at the solution activation. 

Each agent communicates with the appliance through a secured tunnel.

All data is crypted at the source using the appliance's own key. 

This key and all the configurations specific to the appliance are backed up on a regular basis and secured to the second appliance or the Wooko infrastructure to enable the backup continuity and also a disaster recovery on the appliance. 

All data physically stored on the appliance is encrypted, compressed and broken down via the versioning system management, and therefore unusable in the state in case of extraction or physical manipulation on the appliance.

## Technical Components

![](.gitbook/assets/image%20%2835%29.png)

