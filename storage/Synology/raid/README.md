# SNMP Synology raid
Template SNMP Synology raid  made by automate@izi-it
Hash: xxxxxxxxxxxxxxx
## Summary
* [discoveries](#discoveries)
  * [Discovery Synology raid ](#discovery_synology_raid
)
<a name="discoveries" />
## Discoveries

| name | key | type | delay |
| ------------- |------------- |------------- |------------- |
| Synology raid | synoRaidraidName-[{#SNMPVALUE}] | SNMP_AGENT | 1m |

<a name="discovery_synology_raid" />
## Discovery Synology raid

### Items

| name | key | type |
| ------------- |------------- |------------- |
| Raid {#RAID}: Free size | raidFreeSize[{#SNMPINDEX}] | SNMP_AGENT |
| Raid {#RAID}: Total size | raidTotalSize[{#SNMPINDEX}] | SNMP_AGENT |
| Raid {#RAID}: Status | synoRaidraidStatus[{#SNMPINDEX}] | SNMP_AGENT |
