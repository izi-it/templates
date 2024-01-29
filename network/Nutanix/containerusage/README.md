# SNMP Nutanix containerusage
Template SNMP Nutanix by automate@izi-it
Hash: xxxxxxxxxxxxxxx

Template to check SNMP Nutanix containerusage equipments using SNMP protocol
## Summary
* [discoveries](#discoveries)
  * [Discovery Nutanix clusterusage ](#discovery_nutanix_clusterusage
)
<a name="discoveries" />
## Discoveries

| name | key | type | delay |
| ------------- |------------- |------------- |------------- |
| Nutanix clusterusage | clusterName-[{#SNMPVALUE}] | SNMP_AGENT | 5m |

<a name="discovery_nutanix_clusterusage" />
## Discovery Nutanix clusterusage

### Items

| name | key | type |
| ------------- |------------- |------------- |
| Cluster {#CLUSTER_NAME}: Cluster wide average IO operations | clusterIops[{#SNMPINDEX}] | SNMP_AGENT |
| Cluster {#CLUSTER_NAME}: Cluster Latency | clusterLatency[{#SNMPINDEX}] | SNMP_AGENT |
| Cluster {#CLUSTER_NAME}: Status | clusterStatus[{#SNMPINDEX}] | SNMP_AGENT |
| Cluster {#CLUSTER_NAME}: Total storage capacity | clusterTotalStorageCapacity[{#SNMPINDEX}] | SNMP_AGENT |
| Cluster {#CLUSTER_NAME}: Used storage | clusterUsedStorageCapacity[{#SNMPINDEX}] | SNMP_AGENT |
