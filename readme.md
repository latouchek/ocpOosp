### Synopsis

A set of  playbooks to deploy OSC infra on top of OSP. (In progress)

<table>
  <tr>
    <td>Node Type</td>
    <td>Quantity</td>
    <td>vCPU</td>
    <td>RAM</td>
    <td>Storage</td>
    <td>Notes</td>
  </tr>
  <tr>
    <td>LB</td>
    <td>2</td>
    <td>1</td>
    <td>4</td>
    <td>20Gb</td>
    <td>One volume, vda</td>
  </tr>
  <tr>
    <td>Master</td>
    <td>3</td>
    <td>2</td>
    <td>16</td>
    <td>2x50Gb</td>
    <td>Two volumes, vda + vdb</td>
  </tr>
  <tr>
    <td>Infra</td>
    <td>2</td>
    <td>2</td>
    <td>16</td>
    <td>2x50Gb</td>
    <td>Two volumes, vda + vdb</td>
  </tr>
  <tr>
    <td>App</td>
    <td>n</td>
    <td>1</td>
    <td>16</td>
    <td>2x50Gb</td>
    <td>Two volumes, vda + vdb</td>
  </tr>
  <tr>
    <td>Bastion</td>
    <td>1</td>
    <td>1</td>
    <td>4</td>
    <td>30Gb</td>
    <td>One volume, vda</td>
  </tr>
</table>


### Requirements

Install latest version of ansible

### usage

Provide needed infos in all.yaml

Run:

ansible-playbook openshift-infra-providernet.yaml  

or

ansible-playbook openshift-infra-floating.yaml
