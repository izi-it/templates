# SNMP Purestorage stats
Template SNMP Purestorage stats  made by automate@izi-it
Hash: xxxxxxxxxxxxxxx
## Summary
* [discoveries](#discoveries)
  * [Discovery Purestorage stats ](#discovery_purestorage_stats
)
<a name="discoveries" />
## Discoveries

| name | key | type | delay |
| ------------- |------------- |------------- |------------- |
| Purestorage stats | purePerformance-[{#SNMPVALUE}] | SNMP_AGENT | 1m |

<a name="discovery_purestorage_stats" />
## Discovery Purestorage stats

### Items

| name | key | type |
| ------------- |------------- |------------- |
| Disk {#DISKNAME}: Bad Sector | diskBadSector[{#SNMPINDEX}] | SNMP_AGENT |
| Disk {#DISKNAME}: Health status | diskHealthStatus[{#SNMPINDEX}] | SNMP_AGENT |
| Disk {#DISKNAME}: Remain Life | diskRemainLife[{#SNMPINDEX}] | SNMP_AGENT |
| Disk {#DISKNAME}: Temperature | diskTemperature[{#SNMPINDEX}] | SNMP_AGENT |
| Disk {#DISKNAME}: Status | synoDiskdiskStatus[{#SNMPINDEX}] | SNMP_AGENT |
