# SNMP Allied voltage
Template SNMP Allied voltage by automate@izi-it
Hash: xxxxxxxxxxxxxxx

Template to check SNMP Allied equipments using SNMP protocol
## Summary
* [discoveries](#discoveries)
  * [Discovery Allied voltage ](#discovery_allied_voltage
)
<a name="discoveries" />
## Discoveries

| name | key | type | delay |
| ------------- |------------- |------------- |------------- |
| Allied voltage | atEnvMonv2VoltageDescription-[{#SNMPVALUE}] | SNMP_AGENT | 1m |

<a name="discovery_allied_voltage" />
## Discovery Allied voltage

### Items

| name | key | type |
| ------------- |------------- |------------- |
| Voltage {#VOLTAGE}: Current value | atEnvMonv2VoltageCurrent[{#SNMPINDEX}] | SNMP_AGENT |
| Voltage {#VOLTAGE}: Minimum acceptable | atEnvMonv2VoltageLowerThreshold[{#SNMPINDEX}] | SNMP_AGENT |
| Voltage {#VOLTAGE}: Status | atEnvMonv2VoltageStatus[{#SNMPINDEX}] | SNMP_AGENT |
| Voltage {#VOLTAGE}: Maximum acceptable | atEnvMonv2VoltageUpperThreshold[{#SNMPINDEX}] | SNMP_AGENT |
