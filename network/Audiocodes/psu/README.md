# SNMP Audiocodes psu
Template SNMP Audiocodes psu by automate@izi-it
Hash: xxxxxxxxxxxxxxx

Template to check Audiocodes equipments using SNMP protocol
## Summary
* [discoveries](#discoveries)
  * [Discovery Audiocodes psu ](#discovery_audiocodes_psu
)
<a name="discoveries" />
## Discoveries

| name | key | type | delay |
| ------------- |------------- |------------- |------------- |
| Audiocodes psu | acSysPowerSupplyIndex-[{#SNMPVALUE}] | SNMP_AGENT | 5m |

<a name="discovery_audiocodes_psu" />
## Discovery Audiocodes psu

### Items

| name | key | type |
| ------------- |------------- |------------- |
| PSU {#PSU}: Existence | acSysPowerSupplyExistence[{#SNMPINDEX}] | SNMP_AGENT |
| PSU {#PSU}: Severity | acSysPowerSupplySeverity[{#SNMPINDEX}] | SNMP_AGENT |
