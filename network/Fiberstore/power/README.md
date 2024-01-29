# SNMP Fiberstore psu
TemplateSNMP Fiberstore power by automate@izi-it
Hash: xxxxxxxxxxxxxxx

Template to check Fiberstore power equipments using SNMP protocol
## Summary
* [discoveries](#discoveries)
  * [Discovery Fiberstore psu ](#discovery_fiberstore_psu
)
<a name="discoveries" />
## Discoveries

| name | key | type | delay |
| ------------- |------------- |------------- |------------- |
| Fiberstore psu | devMPowerIndex-[{#SNMPVALUE}] | SNMP_AGENT | 5m |

<a name="discovery_fiberstore_psu" />
## Discovery Fiberstore psu

### Items

| name | key | type |
| ------------- |------------- |------------- |
| PSU {#PSU}: Status | devMPowerAlertStatus[{#SNMPINDEX}] | SNMP_AGENT |
