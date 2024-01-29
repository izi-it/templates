# SNMP Redback psu
Template SNMP Redback psu by automate@izi-it
Hash: xxxxxxxxxxxxxxx

Template to check Redback psi equipments using SNMP protocol
## Summary
* [discoveries](#discoveries)
  * [Discovery Redback PSU ](#discovery_redback_psu
)
<a name="discoveries" />
## Discoveries

| name | key | type | delay |
| ------------- |------------- |------------- |------------- |
| Redback PSU | rbnPowerStatusEntry-[{#SNMPVALUE}] | SNMP_AGENT | 1h |

<a name="discovery_redback_psu" />
## Discovery Redback PSU

### Items

| name | key | type |
| ------------- |------------- |------------- |
| PSU {#PSU}: Description | rbnPowerDescr[{#SNMPINDEX}] | SNMP_AGENT |
| PSU {#PSU}: Status | rbnPowerStatus[{#SNMPINDEX}] | SNMP_AGENT |
