# SNMP Synology disk
Template SNMP Synology disk  made by automate@izi-it
Hash: xxxxxxxxxxxxxxx

Check disk
## Summary
* [discoveries](#discoveries)
  * [Discovery Synology disk ](#discovery_synology_disk
)
<a name="discoveries" />
## Discoveries

| name | key | type | delay |
| ------------- |------------- |------------- |------------- |
| Synology disk | synoDiskdiskName-[{#SNMPVALUE}] | SNMP_AGENT | 1m |

<a name="discovery_synology_disk" />
## Discovery Synology disk

### Items

| name | key | type |
| ------------- |------------- |------------- |
| Disk {#DISKNAME}: Bad Sector | diskBadSector[{#SNMPINDEX}] | SNMP_AGENT |
| Disk {#DISKNAME}: Health status | diskHealthStatus[{#SNMPINDEX}] | SNMP_AGENT |
| Disk {#DISKNAME}: Remain Life | diskRemainLife[{#SNMPINDEX}] | SNMP_AGENT |
| Disk {#DISKNAME}: Temperature | diskTemperature[{#SNMPINDEX}] | SNMP_AGENT |
| Disk {#DISKNAME}: Status | synoDiskdiskStatus[{#SNMPINDEX}] | SNMP_AGENT |
