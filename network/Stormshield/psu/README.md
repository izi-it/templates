# SNMP Stormshield psu
Template SNMP Stormshield by automate@izi-it
Hash: xxxxxxxxxxxxxxx

Template to check SNMP Stormshield psu equipments using SNMP protocol
## Summary
* [discoveries](#discoveries)
  * [Discovery Stormshield psu ](#discovery_stormshield_psu
)
<a name="discoveries" />
## Discoveries

| name | key | type | delay |
| ------------- |------------- |------------- |------------- |
| Stormshield psu | snsPowerSupplyPowered-[{#SNMPVALUE}] | SNMP_AGENT | 5m |

<a name="discovery_stormshield_psu" />
## Discovery Stormshield psu

### Items

| name | key | type |
| ------------- |------------- |------------- |
| {#PSU}: Status | snsPowerSupplyStatus[{#SNMPINDEX}] | SNMP_AGENT |
