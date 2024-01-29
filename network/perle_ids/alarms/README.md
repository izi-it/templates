# SNMP Perle ids alarms
Template SNMP Perle ids alarms by automate@izi-it
Hash: xxxxxxxxxxxxxxx

Template to check Perle ids alarms  equipments using SNMP protocol
## Summary
* [discoveries](#discoveries)
  * [Discovery Perle Ids alarms ](#discovery_perle_ids_alarms
)
<a name="discoveries" />
## Discoveries

| name | key | type | delay |
| ------------- |------------- |------------- |------------- |
| Perle Ids alarms | perleEntityAlarmEntry-[{#SNMPVALUE}] | SNMP_AGENT | 1h |

<a name="discovery_perle_ids_alarms" />
## Discovery Perle Ids alarms

### Items

| name | key | type |
| ------------- |------------- |------------- |
| Alarms {#ALARMS}: Description | perleEntityAlarmDescr[{#SNMPINDEX}] | SNMP_AGENT |
| Alarms {#ALARMS}: Severity | perleEntityAlarmSeverity[{#SNMPINDEX}] | SNMP_AGENT |
| Alarms {#ALARMS}: Source Name | perleEntityAlarmSourceName[{#SNMPINDEX}] | SNMP_AGENT |
| Alarms {#ALARMS}: TimeStamp | perleEntityAlarmTimeStamp[{#SNMPINDEX}] | SNMP_AGENT |
