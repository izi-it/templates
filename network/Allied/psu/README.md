# SNMP Allied psu
Template SNMP Allied psu by automate@izi-it
Hash: xxxxxxxxxxxxxxx

Template to check SNMP Allied equipments using SNMP protocol
## Summary
* [discoveries](#discoveries)
  * [Discovery Allied psu ](#discovery_allied_psu
)
<a name="discoveries" />
## Discoveries

| name | key | type | delay |
| ------------- |------------- |------------- |------------- |
| Allied psu | atEnvMonv2PsbSensorDescription-[{#SNMPVALUE}] | SNMP_AGENT | 1m |

<a name="discovery_allied_psu" />
## Discovery Allied psu

### Items

| name | key | type |
| ------------- |------------- |------------- |
| PSU {#PSU}: Status | atEnvMonv2PsbSensorStatus[{#SNMPINDEX}] | SNMP_AGENT |
