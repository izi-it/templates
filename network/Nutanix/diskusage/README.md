# SNMP Nutanix diskusage
Template SNMP Nutanix by automate@izi-it
Hash: xxxxxxxxxxxxxxx

Template to check SNMP Nutanix diskusage equipments using SNMP protocol
## Summary
* [discoveries](#discoveries)
  * [Discovery Nutanix diskusage ](#discovery_nutanix_diskusage
)
<a name="discoveries" />
## Discoveries

| name | key | type | delay |
| ------------- |------------- |------------- |------------- |
| Nutanix diskusage | dstDiskId-[{#SNMPVALUE}] | SNMP_AGENT | 5m |

<a name="discovery_nutanix_diskusage" />
## Discovery Nutanix diskusage

### Items

| name | key | type |
| ------------- |------------- |------------- |
| Disk {#DISK_NAME}: Average Latency | dstAverageLatency[{#SNMPINDEX}] | SNMP_AGENT |
| Disk {#DISK_NAME}: Controller VM ID | dstControllerVMId[{#SNMPINDEX}] | SNMP_AGENT |
| Disk {#DISK_NAME}:  Number IO for the disk | dstNumberIops[{#SNMPINDEX}] | SNMP_AGENT |
| Disk {#DISK_NAME}: Free capacity | dstNumFreeBytes[{#SNMPINDEX}] | SNMP_AGENT |
| Disk {#DISK_NAME}: Free inodes | dstNumFreeInodes[{#SNMPINDEX}] | SNMP_AGENT |
| Disk {#DISK_NAME}: Total capacity | dstNumTotalBytes[{#SNMPINDEX}] | SNMP_AGENT |
| Disk {#DISK_NAME}: Total inodes | dstNumTotalInodes[{#SNMPINDEX}] | SNMP_AGENT |
| Disk {#DISK_NAME}: Disk state | dstState[{#SNMPINDEX}] | SNMP_AGENT |
