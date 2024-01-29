# SNMP Barracuda cloudgen voltage
Template to check SNMP Barracuda cloudgen equipments using SNMP protocol by izi-it
## Summary
* [discoveries](#discoveries)
  * [Discovery Barracuda cloudgen voltage ](#discovery_barracuda_cloudgen_voltage
)
<a name="discoveries" />
## Discoveries

| name | key | type | delay |
| ------------- |------------- |------------- |------------- |
| Barracuda cloudgen voltage | hwSensorName-[{#SNMPVALUE}] | SNMP_AGENT | 1h |

<a name="discovery_barracuda_cloudgen_voltage" />
## Discovery Barracuda cloudgen voltage

### Items

| name | key | type |
| ------------- |------------- |------------- |
| Voltage {#VOLTAGE}: Type | hwSensorType[{#SNMPINDEX}] | SNMP_AGENT |
| Voltage {#VOLTAGE}: Value | hwSensorValue[{#SNMPINDEX}] | SNMP_AGENT |
