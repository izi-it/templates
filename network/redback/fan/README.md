# SNMP Redback fan
Template SNMP Redback fan by automate@izi-it
Hash: xxxxxxxxxxxxxxx

Template to check Redback fan equipments using SNMP protocol
## Summary
* [discoveries](#discoveries)
  * [Discovery Redback Fan ](#discovery_redback_fan
)
<a name="discoveries" />
## Discoveries

| name | key | type | delay |
| ------------- |------------- |------------- |------------- |
| Redback Fan | rbnFanStatusEntry-[{#SNMPVALUE}] | SNMP_AGENT | 1h |

<a name="discovery_redback_fan" />
## Discovery Redback Fan

### Items

| name | key | type |
| ------------- |------------- |------------- |
| Fan {#FAN}: Description | rbnFanDescr[{#SNMPINDEX}] | SNMP_AGENT |
| Fan {#FAN}: Status | rbnFanStatus[{#SNMPINDEX}] | SNMP_AGENT |
