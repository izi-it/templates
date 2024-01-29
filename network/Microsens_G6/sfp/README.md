# SNMP Microsens G6 sfp
Template SNMP Microsens G6 sfp by automate@izi-it
Hash: xxxxxxxxxxxxxxx

Template to check Microsens G6 equipments using SNMP protocol
## Summary
* [discoveries](#discoveries)
  * [Discovery Microsens G6 sfp ](#discovery_microsens_g6_sfp
)
<a name="discoveries" />
## Discoveries

| name | key | type | delay |
| ------------- |------------- |------------- |------------- |
| Microsens G6 sfp | informationPort-[{#SNMPVALUE}] | SNMP_AGENT | 5m |

<a name="discovery_microsens_g6_sfp" />
## Discovery Microsens G6 sfp

### Items

| name | key | type |
| ------------- |------------- |------------- |
| SFP Port {#SFP_PORT}: Location | informationLocation[{#SNMPINDEX}] | SNMP_AGENT |
| SFP Port {#SFP_PORT}: Input Power | informationRxPower[{#SNMPINDEX}] | SNMP_AGENT |
| SFP Port {#SFP_PORT}: State | informationStatus[{#SNMPINDEX}] | SNMP_AGENT |
| SFP Port {#SFP_PORT}: Temperature | informationTemperature[{#SNMPINDEX}] | SNMP_AGENT |
| SFP Port {#SFP_PORT}: Out Power | informationTxPower[{#SNMPINDEX}] | SNMP_AGENT |
