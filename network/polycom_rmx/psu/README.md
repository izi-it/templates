# SNMP Polycom rmx psu
Template SNMP Polycom rmx  psu by automate@izi-it
Hash: xxxxxxxxxxxxxxx

Template to check Polycom rmx psu equipments using SNMP protocol
## Summary
* [discoveries](#discoveries)
  * [Discovery Polycom rmx psu ](#discovery_polycom_rmx_psu
)
<a name="discoveries" />
## Discoveries

| name | key | type | delay |
| ------------- |------------- |------------- |------------- |
| Polycom rmx psu | polycomhardwarepsu-[{#SNMPVALUE}] | SNMP_AGENT | 1h |

<a name="discovery_polycom_rmx_psu" />
## Discovery Polycom rmx psu

### Items

| name | key | type |
| ------------- |------------- |------------- |
| PSU {#PSU}: Status | hardwarePowerSupplyStatus[{#SNMPINDEX}] | SNMP_AGENT |
