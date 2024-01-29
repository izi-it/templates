# SNMP Polycom rmx fan
Template SNMP Polycom rmx fan by automate@izi-it
Hash: xxxxxxxxxxxxxxx

Template to check Polycom rmx fan equipments using SNMP protocol
## Summary
* [discoveries](#discoveries)
  * [Discovery Polycom rmx fan ](#discovery_polycom_rmx_fan
)
<a name="discoveries" />
## Discoveries

| name | key | type | delay |
| ------------- |------------- |------------- |------------- |
| Polycom rmx fan | polycomhardwarefan-[{#SNMPVALUE}] | SNMP_AGENT | 1h |

<a name="discovery_polycom_rmx_fan" />
## Discovery Polycom rmx fan

### Items

| name | key | type |
| ------------- |------------- |------------- |
| Fan {#FAN}: Status | hardwareFanStatus[{#SNMPINDEX}] | SNMP_AGENT |
