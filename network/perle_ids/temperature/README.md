# SNMP Perle ids temperature
Template SNMP Perle ids temperature by automate@izi-it
Hash: xxxxxxxxxxxxxxx

Template to check Perle ids temperature  equipments using SNMP protocol
## Summary
* [discoveries](#discoveries)
  * [Discovery Perle Ids Temperature ](#discovery_perle_ids_temperature
)
<a name="discoveries" />
## Discoveries

| name | key | type | delay |
| ------------- |------------- |------------- |------------- |
| Perle Ids Temperature | perleEnvMonTemperatureStatusEntry-[{#SNMPVALUE}] | SNMP_AGENT | 1h |

<a name="discovery_perle_ids_temperature" />
## Discovery Perle Ids Temperature

### Items

| name | key | type |
| ------------- |------------- |------------- |
| Temperature {#SENSOR}: State | perleEnvMonTemperatureState[{#SNMPINDEX}] | SNMP_AGENT |
| Temperature {#SENSOR}: Description | perleEnvMonTemperatureStatusDescr[{#SNMPINDEX}] | SNMP_AGENT |
| Temperature {#SENSOR}: Current temperature | perleEnvMonTemperatureStatusValue[{#SNMPINDEX}] | SNMP_AGENT |
