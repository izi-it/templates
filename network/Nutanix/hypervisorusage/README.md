# SNMP Nutanix hypervisorusage
Template SNMP Nutanix by automate@izi-it
Hash: xxxxxxxxxxxxxxx

Template to check SNMP Nutanix hypervisorusage equipments using SNMP protocol
## Summary
* [discoveries](#discoveries)
  * [Discovery Nutanix hypervisorusage ](#discovery_nutanix_hypervisorusage
)
<a name="discoveries" />
## Discoveries

| name | key | type | delay |
| ------------- |------------- |------------- |------------- |
| Nutanix hypervisorusage | dstDiskId-[{#SNMPVALUE}] | SNMP_AGENT | 5m |

<a name="discovery_nutanix_hypervisorusage" />
## Discovery Nutanix hypervisorusage

### Items

| name | key | type |
| ------------- |------------- |------------- |
| Hypervisor {#HYPERVISOR_NAME}: Average Latency | hypervisorAverageLatency[{#SNMPINDEX}] | SNMP_AGENT |
| Hypervisor {#HYPERVISOR_NAME}: CPU Usage | hypervisorCpuUsagePercent[{#SNMPINDEX}] | SNMP_AGENT |
| Hypervisor {#HYPERVISOR_NAME}: Memory usage | hypervisorMemoryUsagePercent[{#SNMPINDEX}] | SNMP_AGENT |
| Hypervisor {#HYPERVISOR_NAME}: Avalaible Memory | hypervisorMemory[{#SNMPINDEX}] | SNMP_AGENT |
| Hypervisor {#HYPERVISOR_NAME}: Number of Read IO Operations | hypervisorReadIOPerSecond[{#SNMPINDEX}] | SNMP_AGENT |
| Hypervisor {#HYPERVISOR_NAME}: Number of VM configured | hypervisorVmCount[{#SNMPINDEX}] | SNMP_AGENT |
| Hypervisor {#HYPERVISOR_NAME}: Number of Write IO Operations | hypervisorWriteIOPerSecond[{#SNMPINDEX}] | SNMP_AGENT |
