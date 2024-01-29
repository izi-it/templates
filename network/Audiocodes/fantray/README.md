# SNMP Audiocodes fantray
Template SNMP Audiocodes fantray by automate@izi-it
Hash: xxxxxxxxxxxxxxx

Template to check Audiocodes equipments using SNMP protocol
## Summary
* [discoveries](#discoveries)
  * [Discovery Audiocodes fantray ](#discovery_audiocodes_fantray
)
<a name="discoveries" />
## Discoveries

| name | key | type | delay |
| ------------- |------------- |------------- |------------- |
| Audiocodes fantray | acSysFanTrayIndex-[{#SNMPVALUE}] | SNMP_AGENT | 5m |

<a name="discovery_audiocodes_fantray" />
## Discovery Audiocodes fantray

### Items

| name | key | type |
| ------------- |------------- |------------- |
| Fantray {#FANTRAY_INDEX}: Existence | acSysFanTrayExistence[{#SNMPINDEX}] | SNMP_AGENT |
| Fantray {#FANTRAY_INDEX}: Severity | acSysFanTraySeverity[{#SNMPINDEX}] | SNMP_AGENT |
