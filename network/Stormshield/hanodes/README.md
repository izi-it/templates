# SNMP Stormshield hanodes
Template SNMP Stormshield by automate@izi-it
Hash: xxxxxxxxxxxxxxx

Template to check SNMP Stormshield hanodes equipments using SNMP protocol
## Summary
* [items](#items)
* [discoveries](#discoveries)
  * [Discovery Stormshield hanodes ](#discovery_stormshield_hanodes
)
<a name="items" />
## Items

| name | key | type |
| ------------- |------------- |------------- |
| Number of firewalls registered in the HA cluster but not replying | ntqNbDeadNode | SNMP_AGENT |
| Number of firewalls in the HA cluster | ntqNbNode | SNMP_AGENT |

<a name="discoveries" />
## Discoveries

| name | key | type | delay |
| ------------- |------------- |------------- |------------- |
| Stormshield hanodes | ntqFwSerial-[{#SNMPVALUE}] | SNMP_AGENT | 5m |

<a name="discovery_stormshield_hanodes" />
## Discovery Stormshield hanodes

### Items

| name | key | type |
| ------------- |------------- |------------- |
| {#FW_SERIAL}: HA Licence | ntqHALicence[{#SNMPINDEX}] | SNMP_AGENT |
| {#FW_SERIAL}: HA Quality | ntqHAQuality[{#SNMPINDEX}] | SNMP_AGENT |
| {#FW_SERIAL}: Online | ntqOnline[{#SNMPINDEX}] | SNMP_AGENT |
