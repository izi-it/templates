# SNMP Stormshield health
Template SNMP Stormshield by automate@izi-it
Hash: xxxxxxxxxxxxxxx

Template to check SNMP Stormshield health equipments using SNMP protocol
## Summary
* [discoveries](#discoveries)
  * [Discovery Stormshield health ](#discovery_stormshield_health
)
<a name="discoveries" />
## Discoveries

| name | key | type | delay |
| ------------- |------------- |------------- |------------- |
| Stormshield health | snsSerialHealth-[{#SNMPVALUE}] | SNMP_AGENT | 5m |

<a name="discovery_stormshield_health" />
## Discovery Stormshield health

### Items

| name | key | type |
| ------------- |------------- |------------- |
| {#FW_SERIAL}: Certificate current health status | snsCertHealth[{#SNMPINDEX}] | SNMP_AGENT |
| {#FW_SERIAL}: CPU current health status | snsCPUHealth[{#SNMPINDEX}] | SNMP_AGENT |
| {#FW_SERIAL}: CRLs current health status | snsCRLHealth[{#SNMPINDEX}] | SNMP_AGENT |
| {#FW_SERIAL}: Disk current health status | snsDiskHealth[{#SNMPINDEX}] | SNMP_AGENT |
| {#FW_SERIAL}: Fan current health status | snsFanHealth[{#SNMPINDEX}] | SNMP_AGENT |
| {#FW_SERIAL}: HA Link current health status | snsHaLinkHealth[{#SNMPINDEX}] | SNMP_AGENT |
| {#FW_SERIAL}: Memory current health status | snsMemHealth[{#SNMPINDEX}] | SNMP_AGENT |
| {#FW_SERIAL}: Power supply current health status | snsPowerSupplyHealth[{#SNMPINDEX}] | SNMP_AGENT |
| {#FW_SERIAL}: Raid current health status | snsRaidHealth[{#SNMPINDEX}] | SNMP_AGENT |
