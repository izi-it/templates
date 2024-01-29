# SNMP Barracuda cloudgen fan
Template to check SNMP Barracuda cloudgen equipments using SNMP protocol by izi-it
## Summary
* [discoveries](#discoveries)
  * [Discovery Barracuda cloudgen fan ](#discovery_barracuda_cloudgen_fan
)
<a name="discoveries" />
## Discoveries

| name | key | type | delay |
| ------------- |------------- |------------- |------------- |
| Barracuda cloudgen fan | hwSensorName-[{#SNMPVALUE}] | SNMP_AGENT | 1h |

<a name="discovery_barracuda_cloudgen_fan" />
## Discovery Barracuda cloudgen fan

### Items

| name | key | type |
| ------------- |------------- |------------- |
| Fan {#FAN}: Type | hwSensorType[{#SNMPINDEX}] | SNMP_AGENT |
| Fan {#FAN}: Value | hwSensorValue[{#SNMPINDEX}] | SNMP_AGENT |
