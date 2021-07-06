# SMB/CIFS share connector

{% hint style="info" %}
Only SMB v2 is supported
{% endhint %}

To perform a backup of a windows share \(SMB/CIFS\), no agent installation is required. The agent embedded in the appliance will be used to do the backup.

Upon the activation of the solution, the agent embedded in the appliance is installed, it will have the same hostname as the appliance.

If the agent is not deployed, you can go back to the administration and force its installation.

* Once the agent available, select it:

![](../../.gitbook/assets/image%20%2834%29.png)

* Then go to  "Remote share" on the right:

![](../../.gitbook/assets/menu_remote_share.gif)

* Click "+" to create a new share

![](../../.gitbook/assets/new_share.gif)

It is necessary to specify a share name to identify it easily, a network adress, the point and ID of the mounting \(do not enter the domain, it will be automatically detected\). 

