# SNMP Allied temperature
Template SNMP Allied temperature by automate@izi-it
Hash: xxxxxxxxxxxxxxx

Template to check SNMP Allied equipments using SNMP protocol
## Summary
* [discoveries](#discoveries)
  * [Discovery Allied temperature ](#discovery_allied_temperature
)
<a name="discoveries" />
## Discoveries

| name | key | type | delay |
| ------------- |------------- |------------- |------------- |
| Allied temperature | atEnvMonv2TemperatureDescription-[{#SNMPVALUE}] | SNMP_AGENT | 1m |

<a name="discovery_allied_temperature" />
## Discovery Allied temperature

### Items

| name | key | type |
| ------------- |------------- |------------- |
| Temperature {#TEMPERATURE}: Value | atEnvMonv2TemperatureCurrent[{#SNMPINDEX}] | SNMP_AGENT |
| Temperature {#TEMPERATURE}: Status | atEnvMonv2TemperatureStatus[{#SNMPINDEX}] | SNMP_AGENT |
| Temperature {#TEMPERATURE}: Maximum acceptable | atEnvMonv2TemperatureUpperThreshold[{#SNMPINDEX}] | SNMP_AGENT |
