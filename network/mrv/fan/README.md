# SNMP MRV Optiswitch Fan
No template description
## Summary
* [discoveries](#discoveries)
  * [Discovery Optiswitch fan ](#discovery_optiswitch_fan
)
<a name="discoveries" />
## Discoveries

| name | key | type | delay |
| ------------- |------------- |------------- |------------- |
| Optiswitch fan | FANIndex | SNMP_AGENT | 1m |

<a name="discovery_optiswitch_fan" />
## Discovery Optiswitch fan

### Items

| name | key | type |
| ------------- |------------- |------------- |
| Card Fan {#FAN} : Status | FANOperStatus[{#SNMPINDEX}] | SNMP_AGENT |
