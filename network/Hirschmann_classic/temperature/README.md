# SNMP Hirschmann classic temperature
TemplateSNMP Hirschmann classic temperature made by automate@izi-it
Hash: xxxxxxxxxxxxxxx
## Summary
* [discoveries](#discoveries)
  * [Discovery Hirschmann classic temperature ](#discovery_hirschmann_classic_temperature
)
<a name="discoveries" />
## Discoveries

| name | key | type | delay |
| ------------- |------------- |------------- |------------- |
| Hirschmann classic temperature | hmTempTable-[{#SNMPVALUE}] | SNMP_AGENT | 1m |

<a name="discovery_hirschmann_classic_temperature" />
## Discovery Hirschmann classic temperature

### Items

| name | key | type |
| ------------- |------------- |------------- |
| Temperature {#TEMPERATURE}: Value | hmTemperature[{#SNMPINDEX}] | SNMP_AGENT |
| Temperature {#TEMPERATURE}: Minimum | hmTempLwrLimit[{#SNMPINDEX}] | SNMP_AGENT |
| Temperature {#TEMPERATURE}: Maximum | hmTempUprLimit[{#SNMPINDEX}] | SNMP_AGENT |
