# SNMP Stormshield disk
Template SNMP Stormshield by automate@izi-it
Hash: xxxxxxxxxxxxxxx

Template to check SNMP Stormshield disk equipments using SNMP protocol
## Summary
* [discoveries](#discoveries)
  * [Discovery Stormshield disk ](#discovery_stormshield_disk
)
<a name="discoveries" />
## Discoveries

| name | key | type | delay |
| ------------- |------------- |------------- |------------- |
| Stormshield disk | snsDiskEntryDiskName-[{#SNMPVALUE}] | SNMP_AGENT | 5m |

<a name="discovery_stormshield_disk" />
## Discovery Stormshield disk

### Items

| name | key | type |
| ------------- |------------- |------------- |
| {#DISK_NAME}: Is the disk a member of a RAID | snsDiskEntryIsRaid[{#SNMPINDEX}] | SNMP_AGENT |
| {#DISK_NAME}: RAID Status | snsDiskEntryRaidStatus[{#SNMPINDEX}] | SNMP_AGENT |
