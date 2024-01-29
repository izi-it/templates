# SNMP MRV Optiswitch cpu
No template description
## Summary
* [discoveries](#discoveries)
  * [Discovery Optiswitch cpu ](#discovery_optiswitch_cpu
)
<a name="discoveries" />
## Discoveries

| name | key | type | delay |
| ------------- |------------- |------------- |------------- |
| Optiswitch cpu | CPUIndex | SNMP_AGENT | 1m |

<a name="discovery_optiswitch_cpu" />
## Discovery Optiswitch cpu

### Items

| name | key | type |
| ------------- |------------- |------------- |
| Card CPU {#CPU}: Status | CPUOperStatus[{#SNMPINDEX}] | SNMP_AGENT |
| Card CPU {#CPU}: Redundant mode | CPURedundantMode[{#SNMPINDEX}] | SNMP_AGENT |
