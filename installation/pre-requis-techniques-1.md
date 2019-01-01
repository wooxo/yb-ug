# Pré-requis techniques

## Conditions de fonctionnement

Les appliances doivent être placées dans un environnement adapté au fonctionnement d'un matériel informatique:

* Ne pas exposer au soleil ou à toute flamme 
* Ne pas exposer à tout liquide quel qu'il y soit
* Veiller à maintenir une température ambiante comprise entre 15° et 30° en fonctionnement
* Raccorder l'équipement via l'onduleur \(si fourni\) à un réseau électrique au norme en vigueur 

En cas d'exposition à une flamme ou à tout liquide merci de vous rapprocher au plus tôt du Support Wooxo et ne pas intervenir en autonomie.

Tout fonctionnement "hors-cadre" entrainera une révocation de la garantie.

## Pré-requis réseau

### Communication appliance -&gt; Infrastructure Wooxo/Atempo

L'appliance a besoin de communiquer avec l'infrastructure de Wooxo/Atempo pour récupérer les mises à jour, remonter les alertes et permettre le monitoring des solutions.

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
      <td style="text-align:left">Monitoring matériel</td>
    </tr>
    <tr>
      <td style="text-align:left">46.18.210.130</td>
      <td style="text-align:left">443</td>
      <td style="text-align:left">Activation des licences</td>
    </tr>
    <tr>
      <td style="text-align:left">46.18.210.131</td>
      <td style="text-align:left">443</td>
      <td style="text-align:left">Monitoring logiciel</td>
    </tr>
    <tr>
      <td style="text-align:left">46.18.210.153</td>
      <td style="text-align:left">
        <p>6670 ou</p>
        <p>443 ou</p>
        <p>80 ou</p>
        <p>21 ou</p>
        <p>123 ou</p>
        <p>1720 ou</p>
        <p>1723</p>
      </td>
      <td style="text-align:left">Prise en main maintenance (Support)</td>
    </tr>
    <tr>
      <td style="text-align:left">167.114.245.153</td>
      <td style="text-align:left">6670</td>
      <td style="text-align:left">Brique datacenter YooBackup
        <br />(alertes et externalisation)</td>
    </tr>
    <tr>
      <td style="text-align:left">167.114.240.200</td>
      <td style="text-align:left">
        <p>443 ou</p>
        <p>80 ou</p>
        <p>21 ou</p>
        <p>123 ou</p>
        <p>1720 ou</p>
        <p>1723</p>
      </td>
      <td style="text-align:left">Serveur mise à jour YooBackup</td>
    </tr>
  </tbody>
</table>### Communication appliance -&gt; agent de sauvegarde

La communication utilise le port 6670 en TCP.

### Communication agent de sauvegarde -&gt; appliance ou datacentre

La communication se fait sur le port 6670 en TCP et à l'installation cela nécessite le port  443 en TCP.



