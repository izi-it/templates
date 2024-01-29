# SNMP Redback voltage
Template SNMP Redback voltage  by automate@izi-it
Hash: xxxxxxxxxxxxxxx

Template to check Redback voltage equipments using SNMP protocol
## Summary
* [discoveries](#discoveries)
  * [Discovery Redback Voltage ](#discovery_redback_voltage
)
<a name="discoveries" />
## Discoveries

| name | key | type | delay |
| ------------- |------------- |------------- |------------- |
| Redback Voltage | rbnVoltageSensorEntry-[{#SNMPVALUE}] | SNMP_AGENT | 1h |

<a name="discovery_redback_voltage" />
## Discovery Redback Voltage

### Items

| name | key | type |
| ------------- |------------- |------------- |
| Voltage {#VOLTAGE}: Current voltage level | rbnVoltageCurrent[{#SNMPINDEX}] | SNMP_AGENT |
| Voltage {#VOLTAGE}: Description | rbnVoltageDescr[{#SNMPINDEX}] | SNMP_AGENT |
