# Technical Prerequisites

## Operating Conditions

Appliances must be placed in an environment suitable to hardware working:

* Do not expose to the sun or any flame 
* Do not expose to any liquid
* Make sure the ambiant temperature is between 5° and 50° when operating
* Connect the equipment via the inverter \(if supplied\) to an electrical network that respects the standards in force 

In case of exposition to any flame or liquid, please contact as soon as possible the Wooxo Helpdesk and do not try to intervene by yourself.

Any operation "out of frame" will result in a revocation of the guarantee.

## Network Prerequisites

### Appliance Communication-&gt; Wooxo/Atempo Infrastructure 

The appliance needs to communicate with Wooxo/Atempo infrastructure to collect the last updates, escalate alerts and enable solution monitoring .

<table>
  <thead>
    <tr>
      <th style="text-align:left">IP</th>
      <th style="text-align:left">Port(s) TCP</th>
      <th style="text-align:left">Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">178.33.43.186</td>
      <td style="text-align:left">443</td>
      <td style="text-align:left">Hardware monitoring</td>
    </tr>
    <tr>
      <td style="text-align:left">46.18.210.130</td>
      <td style="text-align:left">443</td>
      <td style="text-align:left">License activation</td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>46.18.210.131 (decommissionned server q1 2019)</p>
        <p>167.114.245.232 (New IP)</p>
      </td>
      <td style="text-align:left">443</td>
      <td style="text-align:left">Software monitoring</td>
    </tr>
    <tr>
      <td style="text-align:left">46.18.210.153</td>
      <td style="text-align:left">
        <p>6670 or</p>
        <p>443 or</p>
        <p>80 or</p>
        <p>21 or</p>
        <p>123 or</p>
        <p>1720 or</p>
        <p>1723</p>
      </td>
      <td style="text-align:left">Getting Started (Support)</td>
    </tr>
    <tr>
      <td style="text-align:left">167.114.245.153</td>
      <td style="text-align:left">6670</td>
      <td style="text-align:left">YooBackup Datacenter brick
        <br />(alerts et outsourcing)</td>
    </tr>
    <tr>
      <td style="text-align:left">167.114.240.200</td>
      <td style="text-align:left">
        <p>443 or</p>
        <p>80 or</p>
        <p>21 or</p>
        <p>123 or</p>
        <p>1720 or</p>
        <p>1723</p>
      </td>
      <td style="text-align:left">YooBackup update server</td>
    </tr>
    <tr>
      <td style="text-align:left">167.114.251.186</td>
      <td style="text-align:left">
        <p>443 or</p>
        <p>80 or</p>
        <p>21 or</p>
        <p>123 or</p>
        <p>1720 or</p>
        <p>1723</p>
      </td>
      <td style="text-align:left">YooBackup secondary update server</td>
    </tr>
  </tbody>
</table>### Appliance Communication -&gt; Backup agent

The communication uses the 6670 port in TCP.

### Backup Agent Communication -&gt; Appliance or Data center

The communication is done on port 6670 in TCP and at the installation the port 443 in TCP is required. 



