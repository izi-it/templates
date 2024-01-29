# SNMP Citrix sdx diskusage
Template SNMP Citrix srx diskusage by automate@izi-it
Hash: xxxxxxxxxxxxxxx

Check disks.
## Summary
* [discoveries](#discoveries)
  * [Discovery Citrix sdx diskusage ](#discovery_citrix_sdx_diskusage
)
<a name="discoveries" />
## Discoveries

| name | key | type | delay |
| ------------- |------------- |------------- |------------- |
| Citrix sdx diskusage | citrixdiskName-[{#SNMPVALUE}] | SNMP_AGENT | 5m |

<a name="discovery_citrix_sdx_diskusage" />
## Discovery Citrix sdx diskusage

### Items

| name | key | type |
| ------------- |------------- |------------- |
| {#DISK_NAME}: Size | diskSize[{#SNMPINDEX}] | SNMP_AGENT |
| {#DISK_NAME}: Total blocks read | diskTotalBlocksRead[{#SNMPINDEX}] | SNMP_AGENT |
| {#DISK_NAME}: Total blocks written | diskTotalBlocksWritten[{#SNMPINDEX}] | SNMP_AGENT |
| {#DISK_NAME}: Utilization | diskUtilized[{#SNMPINDEX}] | SNMP_AGENT |
