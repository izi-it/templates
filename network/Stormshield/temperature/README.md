# SNMP Stormshield temperature
Template SNMP Stormshield by automate@izi-it
Hash: xxxxxxxxxxxxxxx

Template to check SNMP Stormshield temperature equipments using SNMP protocol
## Summary
* [discoveries](#discoveries)
  * [Discovery Stormshield temperature ](#discovery_stormshield_temperature
)
<a name="discoveries" />
## Discoveries

| name | key | type | delay |
| ------------- |------------- |------------- |------------- |
| Stormshield temperature | snsCpuIndex-[{#SNMPVALUE}] | SNMP_AGENT | 5m |

<a name="discovery_stormshield_temperature" />
## Discovery Stormshield temperature

### Items

| name | key | type |
| ------------- |------------- |------------- |
| CPU {#SNMPINDEX}: Temperature  value | snsCpuTemp[{#SNMPINDEX}] | SNMP_AGENT |
