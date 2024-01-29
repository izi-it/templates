# SNMP Stonesoft storage
Template SNMP Stonesoft by automate@izi-it
Hash: xxxxxxxxxxxxxxx

Template to check SNMP Stonesoft storage equipments using SNMP protocol
## Summary
* [discoveries](#discoveries)
  * [Discovery Stonesoft storage ](#discovery_stonesoft_storage
)
<a name="discoveries" />
## Discoveries

| name | key | type | delay |
| ------------- |------------- |------------- |------------- |
| Stonesoft storage | fwMountPointName-[{#SNMPVALUE}] | SNMP_AGENT | 5m |

<a name="discovery_stonesoft_storage" />
## Discovery Stonesoft storage

### Items

| name | key | type |
| ------------- |------------- |------------- |
| {#MOUNTPOINT_NAME}: Free space | fwPartitionAvail[{#SNMPINDEX}] | SNMP_AGENT |
| {#MOUNTPOINT_NAME}: Total size | fwPartitionSize[{#SNMPINDEX}] | SNMP_AGENT |
| {#MOUNTPOINT_NAME}: Used space | fwPartitionUsed[{#SNMPINDEX}] | SNMP_AGENT |
