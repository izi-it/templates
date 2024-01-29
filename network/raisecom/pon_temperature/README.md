# SNMP Raisecom pon temperature
Template SNMP Raisecom pon temperature by automate@izi-it
Hash: xxxxxxxxxxxxxxx

Template to check Raisecom pon temperature equipments using SNMP protocol
## Summary
* [discoveries](#discoveries)
  * [Discovery Raisecom Pon Temperature ](#discovery_raisecom_pon_temperature
)
<a name="discoveries" />
## Discoveries

| name | key | type | delay |
| ------------- |------------- |------------- |------------- |
| Raisecom Pon Temperature | pon_raisecomShelfTemperature-[{#SNMPVALUE}] | SNMP_AGENT | 1h |

<a name="discovery_raisecom_pon_temperature" />
## Discovery Raisecom Pon Temperature

### Items

| name | key | type |
| ------------- |------------- |------------- |
| Temperature {#SENSOR}: Current temperature | pon_raisecomTemperatureValue[{#SNMPINDEX}] | SNMP_AGENT |
