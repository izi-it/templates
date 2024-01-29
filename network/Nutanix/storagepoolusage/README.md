# SNMP Nutanix storagepoolusage
Template SNMP Nutanix by automate@izi-it
Hash: xxxxxxxxxxxxxxx

Template to check SNMP Nutanix storagepoolusage equipments using SNMP protocol
## Summary
* [discoveries](#discoveries)
  * [Discovery Nutanix storagepoolusage ](#discovery_nutanix_storagepoolusage
)
<a name="discoveries" />
## Discoveries

| name | key | type | delay |
| ------------- |------------- |------------- |------------- |
| Nutanix storagepoolusage | spitStoragePoolName-[{#SNMPVALUE}] | SNMP_AGENT | 5m |

<a name="discovery_nutanix_storagepoolusage" />
## Discovery Nutanix storagepoolusage

### Items

| name | key | type |
| ------------- |------------- |------------- |
| Storage Pool{#STORAGEPOOL_NAME}: Average IO latency | spitAvgLatencyUsecs[{#SNMPINDEX}] | SNMP_AGENT |
| Storage Pool{#STORAGEPOOL_NAME}: Number of IO Operations | spitIOPerSecond[{#SNMPINDEX}] | SNMP_AGENT |
| Storage Pool{#STORAGEPOOL_NAME}: Total capacity | spitTotalCapacity[{#SNMPINDEX}] | SNMP_AGENT |
| Storage Pool{#STORAGEPOOL_NAME}: Used capacity | spitUsedCapacity[{#SNMPINDEX}] | SNMP_AGENT |
