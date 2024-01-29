# SNMP Redback temperature
Template SNMP Redback temperature by automate@izi-it
Hash: xxxxxxxxxxxxxxx

Template to check Redback temperature equipments using SNMP protocol
## Summary
* [discoveries](#discoveries)
  * [Discovery Redback Temperature ](#discovery_redback_temperature
)
<a name="discoveries" />
## Discoveries

| name | key | type | delay |
| ------------- |------------- |------------- |------------- |
| Redback Temperature | rbnEntityTempSensorEntry-[{#SNMPVALUE}] | SNMP_AGENT | 1h |

<a name="discovery_redback_temperature" />
## Discovery Redback Temperature

### Items

| name | key | type |
| ------------- |------------- |------------- |
| Temperature {#SENSOR}: Current temperature | rbnEntityTempCurrent[{#SNMPINDEX}] | SNMP_AGENT |
| Temperature {#SENSOR}: Description | rbnEntityTempDescr[{#SNMPINDEX}] | SNMP_AGENT |
