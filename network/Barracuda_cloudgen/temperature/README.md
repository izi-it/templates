# SNMP Barracuda cloudgen temperature
Template to check SNMP Barracuda cloudgen equipments using SNMP protocol by izi-it
## Summary
* [discoveries](#discoveries)
  * [Discovery Barracuda cloudgen temperature ](#discovery_barracuda_cloudgen_temperature
)
<a name="discoveries" />
## Discoveries

| name | key | type | delay |
| ------------- |------------- |------------- |------------- |
| Barracuda cloudgen temperature | hwSensorName-[{#SNMPVALUE}] | SNMP_AGENT | 1h |

<a name="discovery_barracuda_cloudgen_temperature" />
## Discovery Barracuda cloudgen temperature

### Items

| name | key | type |
| ------------- |------------- |------------- |
| Temperature {#TEMPERATURE}: Type | hwSensorType[{#SNMPINDEX}] | SNMP_AGENT |
| Temperature {#TEMPERATURE}: Value | hwSensorValue[{#SNMPINDEX}] | SNMP_AGENT |
