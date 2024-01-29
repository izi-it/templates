# SNMP Nutanix vmusage
Template SNMP Nutanix by automate@izi-it
Hash: xxxxxxxxxxxxxxx

Template to check SNMP Nutanix vmusage equipments using SNMP protocol
## Summary
* [discoveries](#discoveries)
  * [Discovery Nutanix vmusage ](#discovery_nutanix_vmusage
)
<a name="discoveries" />
## Discoveries

| name | key | type | delay |
| ------------- |------------- |------------- |------------- |
| Nutanix vmusage | vmName-[{#SNMPVALUE}] | SNMP_AGENT | 5m |

<a name="discovery_nutanix_vmusage" />
## Discovery Nutanix vmusage

### Items

| name | key | type |
| ------------- |------------- |------------- |
| {#VM_NAME}: Average latency | vmAverageLatency[{#SNMPINDEX}] | SNMP_AGENT |
| {#VM_NAME}: CPU Usage | vmCpuUsagePercent[{#SNMPINDEX}] | SNMP_AGENT |
| {#VM_NAME}: Memory Usage | vmMemoryUsagePercent[{#SNMPINDEX}] | SNMP_AGENT |
| {#VM_NAME}: Available Memory | vmMemory[{#SNMPINDEX}] | SNMP_AGENT |
| {#VM_NAME}: Power state of the VM | vmPowerState[{#SNMPINDEX}] | SNMP_AGENT |
| {#VM_NAME}: Number of read io operations | vmReadIOPerSecond[{#SNMPINDEX}] | SNMP_AGENT |
| {#VM_NAME}: Total number of bytes received | vmRxBytes[{#SNMPINDEX}] | SNMP_AGENT |
| {#VM_NAME}: Total number of bytes transmitted | vmTxBytes[{#SNMPINDEX}] | SNMP_AGENT |
| {#VM_NAME}: Number of write io operations | vmWriteIOPerSecond[{#SNMPINDEX}] | SNMP_AGENT |
