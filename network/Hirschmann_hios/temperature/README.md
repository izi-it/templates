# SNMP Hirschmann hios temperature
TemplateSNMP Hirschmann hios temperature made by automate@izi-it
Hash: xxxxxxxxxxxxxxx
## Summary
* [discoveries](#discoveries)
  * [Discovery Hirschmann hios temperature ](#discovery_hirschmann_hios_temperature
)
<a name="discoveries" />
## Discoveries

| name | key | type | delay |
| ------------- |------------- |------------- |------------- |
| Hirschmann hios temperature | hm2DeviceMgmtTemperatureGroup-[{#SNMPVALUE}] | SNMP_AGENT | 1m |

<a name="discovery_hirschmann_hios_temperature" />
## Discovery Hirschmann hios temperature

### Items

| name | key | type |
| ------------- |------------- |------------- |
| Temperature {#TEMPERATURE}: Minimum | hm2DevMgmtTemperatureLowerLimit[{#SNMPINDEX}] | SNMP_AGENT |
| Temperature {#TEMPERATURE}: Maximum | hm2DevMgmtTemperatureUpperLimit[{#SNMPINDEX}] | SNMP_AGENT |
| Temperature {#TEMPERATURE}: Value | hm2DevMgmtTemperature[{#SNMPINDEX}] | SNMP_AGENT |
