# SNMP Citrix netscaler CPU
No template description
## Summary
* [items](#items)
* [discoveries](#discoveries)
  * [Discovery Netscaler cpu ](#discovery_netscaler_cpu
)
<a name="items" />
## Items

| name | key | type |
| ------------- |------------- |------------- |
| Number of CPUs | numCPUs | SNMP_AGENT |

<a name="discoveries" />
## Discoveries

| name | key | type | delay |
| ------------- |------------- |------------- |------------- |
| Netscaler cpu | cpuusage-[{#SNMPVALUE}] | SNMP_AGENT | 1m |

<a name="discovery_netscaler_cpu" />
## Discovery Netscaler cpu

### Items

| name | key | type |
| ------------- |------------- |------------- |
| CPU {#CPU} Usage | cpuusage[{#SNMPINDEX}] | SNMP_AGENT |
