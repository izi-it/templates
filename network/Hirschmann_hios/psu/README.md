# SNMP Hirschmann hios psu
Template SNMP Hirschmann hios psu made by automate@izi-it
Hash: xxxxxxxxxxxxxxx
## Summary
* [discoveries](#discoveries)
  * [Discovery Hirschmann hios psu ](#discovery_hirschmann_hios_psu
)
<a name="discoveries" />
## Discoveries

| name | key | type | delay |
| ------------- |------------- |------------- |------------- |
| Hirschmann hios psu | hm2PSID-[{#SNMPVALUE}] | SNMP_AGENT | 1m |

<a name="discovery_hirschmann_hios_psu" />
## Discovery Hirschmann hios psu

### Items

| name | key | type |
| ------------- |------------- |------------- |
| PSU {#PSU}: State | hm2PSState[{#SNMPINDEX}] | SNMP_AGENT |
