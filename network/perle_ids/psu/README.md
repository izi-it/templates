# SNMP Perle ids  psu
Template SNMP Perle ids psu by automate@izi-it
Hash: xxxxxxxxxxxxxxx

Template to check Perle ids psu  equipments using SNMP protocol
## Summary
* [discoveries](#discoveries)
  * [Discovery Perle Ids PSU ](#discovery_perle_ids_psu
)
<a name="discoveries" />
## Discoveries

| name | key | type | delay |
| ------------- |------------- |------------- |------------- |
| Perle Ids PSU | perleEnvMonPowerSupplyStatusEntry-[{#SNMPVALUE}] | SNMP_AGENT | 1h |

<a name="discovery_perle_ids_psu" />
## Discovery Perle Ids PSU

### Items

| name | key | type |
| ------------- |------------- |------------- |
| PSU {#PSU}: Status | perleEnvMonPowerSupplyState[{#SNMPINDEX}] | SNMP_AGENT |
| PSU {#PSU}: Description | perleEnvMonPowerSupplyStatusDescr[{#SNMPINDEX}] | SNMP_AGENT |
