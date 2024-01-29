# SNMP Netgear Sseries fan
Template SNMP Netgear Sseries fan by automate@izi-it
Hash: xxxxxxxxxxxxxxx

Template to check SNMP Netgear Sseries equipments using SNMP protocol
## Summary
* [discoveries](#discoveries)
  * [Discovery Netgear Sseries fan ](#discovery_netgear_sseries_fan
)
<a name="discoveries" />
## Discoveries

| name | key | type | delay |
| ------------- |------------- |------------- |------------- |
| Netgear Sseries fan | boxServicesFansEntry-[{#SNMPVALUE}] | SNMP_AGENT | 1m |

<a name="discovery_netgear_sseries_fan" />
## Discovery Netgear Sseries fan

### Items

| name | key | type |
| ------------- |------------- |------------- |
| {#FAN}: Fan state | boxServicesFanItemState[{#SNMPINDEX}] | SNMP_AGENT |
| {#FAN}: Fan speed | boxServicesFanSpeed[{#SNMPINDEX}] | SNMP_AGENT |
