# SNMP Stormshield fan
Template SNMP Stormshield by automate@izi-it
Hash: xxxxxxxxxxxxxxx

Template to check SNMP Stormshield fan equipments using SNMP protocol
## Summary
* [discoveries](#discoveries)
  * [Discovery Stormshield fan ](#discovery_stormshield_fan
)
<a name="discoveries" />
## Discoveries

| name | key | type | delay |
| ------------- |------------- |------------- |------------- |
| Stormshield fan | snsFanName-[{#SNMPVALUE}] | SNMP_AGENT | 5m |

<a name="discovery_stormshield_fan" />
## Discovery Stormshield fan

### Items

| name | key | type |
| ------------- |------------- |------------- |
| {#FAN}: Speed | snsFanRpm[{#SNMPINDEX}] | SNMP_AGENT |
| {#FAN}: Status | snsFanStatus[{#SNMPINDEX}] | SNMP_AGENT |
