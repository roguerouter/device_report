# Device Facts, Report Generator

This is a repository containing all the files used to create the network automation series on CML using Ansible.  The output creates a structure as seen below
and works for both NXOS and IOS-XE platforms.  It is a sample of how to use the ios_facts and nxos_facts modules to capture device data, and parse the data through
a Jinja2 template to create an easy to parse YAML file for each device.  It will also capture trunk interfaces, and interfaces with secondary IPs.  However it is
unable to capture dot1q encapsulated interfaces at this time.

```
Hostname: 
Device Type: 
Model: 
Serial: 
Version: 
Interfaces: 
- Name: 
  Description: 
  Enabled: 
  IP_address: 
  Mode: 
  VLAN:
VLAN_List:
- VLAN_ID:
```
