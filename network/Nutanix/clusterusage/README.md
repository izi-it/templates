# SNMP Nutanix clusterusage
Template SNMP Nutanix by automate@izi-it
Hash: xxxxxxxxxxxxxxx

Template to check SNMP Nutanix clusterusage equipments using SNMP protocol
## Summary
* [discoveries](#discoveries)
  * [Discovery Nutanix containerusage ](#discovery_nutanix_containerusage
)
<a name="discoveries" />
## Discoveries

| name | key | type | delay |
| ------------- |------------- |------------- |------------- |
| Nutanix containerusage | citContainerName-[{#SNMPVALUE}] | SNMP_AGENT | 5m |

<a name="discovery_nutanix_containerusage" />
## Discovery Nutanix containerusage

### Items

| name | key | type |
| ------------- |------------- |------------- |
| CONTAINER {#CONTAINER_NAME}: Average IO Latency | citAvgLatencyUsecs[{#SNMPINDEX}] | SNMP_AGENT |
| CONTAINER {#CONTAINER_NAME}: Number of IO Operations | citIOPerSecond[{#SNMPINDEX}] | SNMP_AGENT |
| CONTAINER {#CONTAINER_NAME}: Total capacity | citTotalCapacity[{#SNMPINDEX}] | SNMP_AGENT |
| CONTAINER {#CONTAINER_NAME}: Used capacity | citUsedCapacity[{#SNMPINDEX}] | SNMP_AGENT |
