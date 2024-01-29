# SNMP Checkpoint voltage
Template to check Checkpoint voltage equipments using SNMP protocol by izi-it
## Summary
* [discoveries](#discoveries)
  * [Discovery Checkpoint voltage ](#discovery_checkpoint_voltage
)
<a name="discoveries" />
## Discoveries

| name | key | type | delay |
| ------------- |------------- |------------- |------------- |
| Checkpoint voltage | voltageSensorEntry-[{#SNMPVALUE}] | SNMP_AGENT | 1h |

<a name="discovery_checkpoint_voltage" />
## Discovery Checkpoint voltage

### Items

| name | key | type |
| ------------- |------------- |------------- |
| Voltage {#VOLTAGE}: Status | voltageSensorStatus[{#SNMPINDEX}] | SNMP_AGENT |
| Voltage {#VOLTAGE}: Value | voltageSensorValue[{#SNMPINDEX}] | SNMP_AGENT |

### Triggers

| name | expression | priority |
| ------------- |------------- |------------- |
| {#VOLTAGE}: Voltage is above the critical threshold | last(/SNMP Checkpoint voltage/voltageSensorStatus[{#SNMPINDEX}])<>0 | HIGH |
