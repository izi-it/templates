# SNMP Allied fan
Template SNMP Allied fan by automate@izi-it
Hash: xxxxxxxxxxxxxxx

Template to check SNMP Allied equipments using SNMP protocol
## Summary
* [discoveries](#discoveries)
  * [Discovery Allied fan ](#discovery_allied_fan
)
<a name="discoveries" />
## Discoveries

| name | key | type | delay |
| ------------- |------------- |------------- |------------- |
| Allied fan | atEnvMonv2FanDescription-[{#SNMPVALUE}] | SNMP_AGENT | 1m |

<a name="discovery_allied_fan" />
## Discovery Allied fan

### Items

| name | key | type |
| ------------- |------------- |------------- |
| Fan {#FAN}: Speed | atEnvMonv2FanCurrentSpeed[{#SNMPINDEX}] | SNMP_AGENT |
| Fan {#FAN}: Minimum acceptable speed | atEnvMonv2FanLowerThreshold[{#SNMPINDEX}] | SNMP_AGENT |
| Fan {#FAN}: Status | atEnvMonv2FanStatus[{#SNMPINDEX}] | SNMP_AGENT |
