# SNMP Fiberstore slot
TemplateSNMP Fiberstore slot by automate@izi-it
Hash: xxxxxxxxxxxxxxx

Template to check Fiberstore slot equipments using SNMP protocol
## Summary
* [discoveries](#discoveries)
  * [Discovery Fiberstore slot ](#discovery_fiberstore_slot
)
<a name="discoveries" />
## Discoveries

| name | key | type | delay |
| ------------- |------------- |------------- |------------- |
| Fiberstore slot | lswSlotIndex-[{#SNMPVALUE}] | SNMP_AGENT | 5m |

<a name="discovery_fiberstore_slot" />
## Discovery Fiberstore slot

### Items

| name | key | type |
| ------------- |------------- |------------- |
| Slot {#SLOT}: Status | lswSlotStatus[{#SNMPINDEX}] | SNMP_AGENT |
