# SNMP Checkpoint fan
Template to check Checkpoint fan equipments using SNMP protocol by izi-it
## Summary
* [discoveries](#discoveries)
  * [Discovery Checkpoint fan ](#discovery_checkpoint_fan
)
<a name="discoveries" />
## Discoveries

| name | key | type | delay |
| ------------- |------------- |------------- |------------- |
| Checkpoint fan | fanSpeedSensorEntry-[{#SNMPVALUE}] | SNMP_AGENT | 1h |

<a name="discovery_checkpoint_fan" />
## Discovery Checkpoint fan

### Items

| name | key | type |
| ------------- |------------- |------------- |
| Fan {#FAN}: Name | fanSpeedSensorName[{#SNMPINDEX}] | SNMP_AGENT |
| Fan {#FAN}: Status | fanSpeedSensorStatus[{#SNMPINDEX}] | SNMP_AGENT |
| Fan {#FAN}: Value | fanSpeedSensorValue[{#SNMPINDEX}] | SNMP_AGENT |

### Triggers

| name | expression | priority |
| ------------- |------------- |------------- |
| Checkpoint : Fan {#FAN} is in critical state | last(/SNMP Checkpoint fan/fanSpeedSensorStatus[{#SNMPINDEX}])<> 0 | AVERAGE |
