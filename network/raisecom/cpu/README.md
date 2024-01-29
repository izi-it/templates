# SNMP Raisecom pon cpu
Template SNMP Raisecom pon cpu by automate@izi-it
Hash: xxxxxxxxxxxxxxx

Template to check Raisecom pon cpu equipments using SNMP protocol
## Summary
* [discoveries](#discoveries)
  * [Discovery Raisecom PON CPU ](#discovery_raisecom_pon_cpu
)
<a name="discoveries" />
## Discoveries

| name | key | type | delay |
| ------------- |------------- |------------- |------------- |
| Raisecom PON CPU | pon_raisecomCPUUtilizationEntry-[{#SNMPVALUE}] | SNMP_AGENT | 1h |

<a name="discovery_raisecom_pon_cpu" />
## Discovery Raisecom PON CPU

### Items

| name | key | type |
| ------------- |------------- |------------- |
| {#PONCPU_UTILIZATION}: CPU Usage 1Second | rcCpuUsage1Second[{#SNMPINDEX}] | SNMP_AGENT |
| {#PONCPU_UTILIZATION}: Cpu Usage 2Hours | rcCpuUsage2Hours[{#SNMPINDEX}] | SNMP_AGENT |
| {#PONCPU_UTILIZATION}: Cpu Usage 10Minutes | rcCpuUsage10Minutes[{#SNMPINDEX}] | SNMP_AGENT |
