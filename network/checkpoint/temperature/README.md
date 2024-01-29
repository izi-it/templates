# SNMP Checkpoint temperature
Template to check Checkpoint temperature equipments using SNMP protocol by izi-it
## Summary
* [discoveries](#discoveries)
  * [Discovery Checkpoint temperature ](#discovery_checkpoint_temperature
)
<a name="discoveries" />
## Discoveries

| name | key | type | delay |
| ------------- |------------- |------------- |------------- |
| Checkpoint temperature | temperatureSensorEntry-[{#SNMPVALUE}] | SNMP_AGENT | 5m |

<a name="discovery_checkpoint_temperature" />
## Discovery Checkpoint temperature

### Items

| name | key | type |
| ------------- |------------- |------------- |
| Temperature Sensor {#TEMPERATURE}: Status | temperatureSensorStatus[{#SNMPINDEX}] | SNMP_AGENT |
| Temperature Sensor {#TEMPERATURE}: Value | temperatureSensorValue[{#SNMPINDEX}] | SNMP_AGENT |

### Triggers

| name | expression | priority |
| ------------- |------------- |------------- |
| {#TEMPERATURE}: Temperature is above critical threshold ({$_CRITTEMP}°C) | last(/SNMP Checkpoint temperature/temperatureSensorStatus[{#SNMPINDEX}])<>0<br>or<br>last(/SNMP Checkpoint temperature/temperatureSensorValue[{#SNMPINDEX}])> {$_CRITTEMP} | HIGH |
| {#TEMPERATURE}: Temperature is above warning threshold ({$_WARNTEMP}°C) | last(/SNMP Checkpoint temperature/temperatureSensorValue[{#SNMPINDEX}])> {$_WARNTEMP}<br>and <br>last(/SNMP Checkpoint temperature/temperatureSensorValue[{#SNMPINDEX}])< {$_CRITTEMP} | WARNING |
