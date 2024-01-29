# SNMP Barracuda cloudgen psu
Template to check SNMP Barracuda cloudgen equipments using SNMP protocol by izi-it
## Summary
* [discoveries](#discoveries)
  * [Discovery Barracuda cloudgen psu ](#discovery_barracuda_cloudgen_psu
)
<a name="discoveries" />
## Discoveries

| name | key | type | delay |
| ------------- |------------- |------------- |------------- |
| Barracuda cloudgen psu | hwSensorName-[{#SNMPVALUE}] | SNMP_AGENT | 1h |

<a name="discovery_barracuda_cloudgen_psu" />
## Discovery Barracuda cloudgen psu

### Items

| name | key | type |
| ------------- |------------- |------------- |
| PSU {#PSU}: Type | hwSensorType[{#SNMPINDEX}] | SNMP_AGENT |
| PSU {#PSU}: Value | hwSensorValue[{#SNMPINDEX}] | SNMP_AGENT |
