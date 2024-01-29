# SNMP Citrix netscaler Disk
No template description
## Summary
* [discoveries](#discoveries)
  * [Discovery Netscaler disk ](#discovery_netscaler_disk
)
<a name="discoveries" />
## Discoveries

| name | key | type | delay |
| ------------- |------------- |------------- |------------- |
| Netscaler disk | sysHealthDiskName-[{#SNMPVALUE}] | SNMP_AGENT | 1m |

<a name="discovery_netscaler_disk" />
## Discovery Netscaler disk

### Items

| name | key | type |
| ------------- |------------- |------------- |
| Disk {#DISK}: Size | sysHealthDiskSize[{#SNMPINDEX}] | SNMP_AGENT |
| Disk {#DISK}: Used | sysHealthDiskUsed[{#SNMPINDEX}] | SNMP_AGENT |
