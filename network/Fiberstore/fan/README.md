# SNMP Fiberstore fan
TemplateSNMP Fiberstore fan by automate@izi-it
Hash: xxxxxxxxxxxxxxx

Template to check Fiberstore fan equipments using SNMP protocol
## Summary
* [discoveries](#discoveries)
  * [Discovery Fiberstore fan ](#discovery_fiberstore_fan
)
<a name="discoveries" />
## Discoveries

| name | key | type | delay |
| ------------- |------------- |------------- |------------- |
| Fiberstore fan | devMFanIndex-[{#SNMPVALUE}] | SNMP_AGENT | 5m |

<a name="discovery_fiberstore_fan" />
## Discovery Fiberstore fan

### Items

| name | key | type |
| ------------- |------------- |------------- |
| Fan {#FAN}: Speed | devMFanSpeed[{#SNMPINDEX}] | SNMP_AGENT |
| Fan {#FAN}: Status | devMFanStatus[{#SNMPINDEX}] | SNMP_AGENT |
