# SNMP Checkpoint psu
Template to check Checkpoint psu equipments using SNMP protocol by izi-it
## Summary
* [discoveries](#discoveries)
  * [Discovery Checkpoint psu ](#discovery_checkpoint_psu
)
<a name="discoveries" />
## Discoveries

| name | key | type | delay |
| ------------- |------------- |------------- |------------- |
| Checkpoint psu | powerSupplyStatus-[{#SNMPVALUE}] | SNMP_AGENT | 1h |

<a name="discovery_checkpoint_psu" />
## Discovery Checkpoint psu

### Items

| name | key | type |
| ------------- |------------- |------------- |
| PSU {#PSU}: Status | powerSupplyStatus[{#SNMPINDEX}] | SNMP_AGENT |

### Triggers

| name | expression | priority |
| ------------- |------------- |------------- |
| {#PSU}:: Power supply is in critical state | last(/SNMP Checkpoint psu/powerSupplyStatus[{#SNMPINDEX}])<>"Up" | HIGH |
