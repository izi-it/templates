# 3Com Generic CPU by SNMP
3Com Generic CPU by SNMP by IZI-IT
## Summary
* [discoveries](#discoveries)
  * [Discovery CPU discovery ](#discovery_cpu_discovery
)
<a name="discoveries" />
## Discoveries

| name | key | type | delay |
| ------------- |------------- |------------- |------------- |
| CPU discovery | cpu.discovery | SNMP_AGENT | 1h |

<a name="discovery_cpu_discovery" />
## Discovery CPU discovery

### Items

| name | key | type |
| ------------- |------------- |------------- |
| {#SNMPVALUE}: CPU percent last 5s | cpu.percent5s[{#SNMPINDEX}] | SNMP_AGENT |
| {#SNMPVALUE}: CPU percent per 1 min | cpu.percent_per1min[{#SNMPINDEX}] | SNMP_AGENT |
| {#SNMPVALUE}: CPU percent per 5 min | cpu.percent_per5min[{#SNMPINDEX}] | SNMP_AGENT |
