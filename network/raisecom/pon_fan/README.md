# SNMP Raisecom pon fan
Template SNMP Raisecom pon fan by automate@izi-it
Hash: xxxxxxxxxxxxxxx

Template to check Raisecom pon fan equipments using SNMP protocol
## Summary
* [discoveries](#discoveries)
  * [Discovery Raisecom PON Fan ](#discovery_raisecom_pon_fan
)
<a name="discoveries" />
## Discoveries

| name | key | type | delay |
| ------------- |------------- |------------- |------------- |
| Raisecom PON Fan | pon_raisecomFanMonitorStateEntry-[{#SNMPVALUE}] | SNMP_AGENT | 1h |

<a name="discovery_raisecom_pon_fan" />
## Discovery Raisecom PON Fan

### Items

| name | key | type |
| ------------- |------------- |------------- |
| Pon Fan {#PON_FAN}: Speed value | pon_raisecomFanSpeedValue[{#SNMPINDEX}] | SNMP_AGENT |
| Pon Fan {#PON_FAN}: Current state | pon_raisecomFanWorkState[{#SNMPINDEX}] | SNMP_AGENT |
