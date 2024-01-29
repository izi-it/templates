# SNMP Raisecom temperature
Template SNMP Raisecom temperature by automate@izi-it
Hash: xxxxxxxxxxxxxxx

Template to check Raisecom temperature equipments using SNMP protocol
## Summary
* [discoveries](#discoveries)
  * [Discovery Raisecom Temperature ](#discovery_raisecom_temperature
)
<a name="discoveries" />
## Discoveries

| name | key | type | delay |
| ------------- |------------- |------------- |------------- |
| Raisecom Temperature | raisecomTemperatureEntry-[{#SNMPVALUE}] | SNMP_AGENT | 1h |

<a name="discovery_raisecom_temperature" />
## Discovery Raisecom Temperature

### Items

| name | key | type |
| ------------- |------------- |------------- |
| Temperature {#SENSOR}: High threshold of the temperature alarm. | raisecomTemperatureThresholdHigh[{#SNMPINDEX}] | SNMP_AGENT |
| Temperature {#SENSOR}: Low threshold of the temperature alarm | raisecomTemperatureThresholdLow[{#SNMPINDEX}] | SNMP_AGENT |
| Temperature {#SENSOR}: Current temperature | raisecomTemperatureValue[{#SNMPINDEX}] | SNMP_AGENT |
