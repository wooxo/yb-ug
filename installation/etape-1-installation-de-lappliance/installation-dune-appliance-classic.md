# Classic Appliance Installation

The Classic appliance installation is easy but must be performed correctly to ensure proper operation. 

## Overview

### Classic Box

![](../../.gitbook/assets/image%20%281%29.png)

### Platinum Connector <a id="platinum-connector"></a>

![](../../.gitbook/assets/image%20%2815%29.png)

## Box Content

* A Classic appliance
* A power rope \(or an external power supply depending on the model, e.g., . [Technical Specifications](https://docs.yoobackup.fr/~/edit/drafts/-LWjtVvwDwbXk_mJzQSr/v/english/specifications-techniques)\)
* A cable RJ45
* An inverter and a specific USB cable
* OneKey Restore USB key

## Electrical Connection

We can now proceed to the electrical connection of the solution:

1. Connect the box to the inverter \(provided with the box depending on the chosen offer\)
2. Connect the inverter USB cable to any USB port of the appliance
3. Connect the inverter to the customer's power grid

## Network Connection

Each appliance has two network ports that can be used to associate it to two physical networks present in the installation.

The default port is indicated by a LAN sticker. If it is not the case, it is the port closest to the power port. 

Once the appliance physically connected to the customer's network, it must be accessible.  For that, 3 solutions:

1. If there is a DHCP and propagation of hostnames, the workstation will be available on the "wooxo-desktop" hostname.
2. You can use WTool which is an utility created by Wooxo \([downloadable here](https://www.wooxo.fr/WTool)\), pay attention if multiple appliances are connected. 
3. Directely from the appliance using a keyboard/screen and a maintenance account \(ID: config/password: config\).

![](../../.gitbook/assets/image%20%2811%29.png)

