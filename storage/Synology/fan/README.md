# SNMP Synology fan
Template SNMP Synology fan  made by automate@izi-it
Hash: xxxxxxxxxxxxxxx
## Summary
* [discoveries](#discoveries)
  * [Discovery Synology fan ](#discovery_synology_fan
)
<a name="discoveries" />
## Discoveries

| name | key | type | delay |
| ------------- |------------- |------------- |------------- |
| Synology fan | synologyfan-[{#SNMPVALUE}] | SNMP_AGENT | 1m |

<a name="discovery_synology_fan" />
## Discovery Synology fan

### Items

| name | key | type |
| ------------- |------------- |------------- |
| CPU Fan {#FAN}: Status | synoSystemcpuFanStatus[{#SNMPINDEX}] | SNMP_AGENT |
| System Fan {#FAN}: Status | synoSystemsystemFanStatus[{#SNMPINDEX}] | SNMP_AGENT |
