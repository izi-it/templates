# SNMP Redback disk
Template SNMP Redback disk by automate@izi-it
Hash: xxxxxxxxxxxxxxx

Template to check Redback diskequipments using SNMP protocol
## Summary
* [discoveries](#discoveries)
  * [Discovery Redback Disk ](#discovery_redback_disk
)
<a name="discoveries" />
## Discoveries

| name | key | type | delay |
| ------------- |------------- |------------- |------------- |
| Redback Disk | rbnSRStorageEntry-[{#SNMPVALUE}] | SNMP_AGENT | 1h |

<a name="discovery_redback_disk" />
## Discovery Redback Disk

### Items

| name | key | type |
| ------------- |------------- |------------- |
| Storage device {#STORAGE_DEVICE}: Description | rbnSRStorageDescr[{#SNMPINDEX}] | SNMP_AGENT |
| Storage device {#STORAGE_DEVICE}: Total Size | rbnSRStorageSize[{#SNMPINDEX}] | SNMP_AGENT |
| Storage device {#STORAGE_DEVICE}:  Status | rbnSRStorageStatus[{#SNMPINDEX}] | SNMP_AGENT |
| Storage device {#STORAGE_DEVICE}: Percent utilization | rbnSRStorageUtilization[{#SNMPINDEX}] | SNMP_AGENT |
