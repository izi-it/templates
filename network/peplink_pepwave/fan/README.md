# SNMP Peplink pepwave wanusage
Template SNMP Peplink pepwave wanusage by automate@izi-it
Hash: xxxxxxxxxxxxxxx

Template to check Peplink pepwave wanusage equipments using SNMP protocol
## Summary
* [discoveries](#discoveries)
  * [Discovery Peplink wave wandatausage ](#discovery_peplink_wave_wandatausage
)  * [Discovery Peplink wave wan ](#discovery_peplink_wave_wan
)
<a name="discoveries" />
## Discoveries

| name | key | type | delay |
| ------------- |------------- |------------- |------------- |
| Peplink wave wandatausage | wanDataUsageEntry-[{#SNMPVALUE}] | SNMP_AGENT | 1h |
| Peplink wave wan | wanEntry-[{#SNMPVALUE}] | SNMP_AGENT | 1h |

<a name="discovery_peplink_wave_wandatausage" />
## Discovery Peplink wave wandatausage

### Items

| name | key | type |
| ------------- |------------- |------------- |
| Wan {#WAN}: Wan network received bytes | wanDataUsageRxByte[{#SNMPINDEX}] | SNMP_AGENT |
| Wan {#WAN}: Wan network transmitted bytes | wanDataUsageTxByte[{#SNMPINDEX}] | SNMP_AGENT |

<a name="discovery_peplink_wave_wan" />
## Discovery Peplink wave wan

### Items

| name | key | type |
| ------------- |------------- |------------- |
| Wan {#WAN}: Health Check State | wanHealthCheckState[{#SNMPINDEX}] | SNMP_AGENT |
| Wan {#WAN} | wanName[{#SNMPINDEX}] | SNMP_AGENT |
| Wan {#WAN}: Signal | wanSignal[{#SNMPINDEX}] | SNMP_AGENT |
