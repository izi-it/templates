# SNMP Raisecom fan
Template SNMP Raisecom fan by automate@izi-it
Hash: xxxxxxxxxxxxxxx

Template to check Raisecom fan equipments using SNMP protocol
## Summary
* [discoveries](#discoveries)
  * [Discovery Raisecom Fan ](#discovery_raisecom_fan
)
<a name="discoveries" />
## Discoveries

| name | key | type | delay |
| ------------- |------------- |------------- |------------- |
| Raisecom Fan | raisecomFanMonitorStateEntry-[{#SNMPVALUE}] | SNMP_AGENT | 1h |

<a name="discovery_raisecom_fan" />
## Discovery Raisecom Fan

### Items

| name | key | type |
| ------------- |------------- |------------- |
| Fan {#FAN}: Speed value | raisecomFanSpeedValue[{#SNMPINDEX}] | SNMP_AGENT |
| Fan {#FAN}: Current state | raisecomFanWorkState[{#SNMPINDEX}] | SNMP_AGENT |
