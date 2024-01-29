# SNMP Audiocodes trunkstatus
Template SNMP Audiocodes trunkstatusby automate@izi-it
Hash: xxxxxxxxxxxxxxx

Template to check Audiocodes trunkstatus equipments using SNMP protocol
## Summary
* [discoveries](#discoveries)
  * [Discovery Audiocodes trunkstatus ](#discovery_audiocodes_trunkstatus
)
<a name="discoveries" />
## Discoveries

| name | key | type | delay |
| ------------- |------------- |------------- |------------- |
| Audiocodes trunkstatus | acTrunkName-[{#SNMPVALUE}] | SNMP_AGENT | 5m |

<a name="discovery_audiocodes_trunkstatus" />
## Discovery Audiocodes trunkstatus

### Items

| name | key | type |
| ------------- |------------- |------------- |
| Trunk {#TRUNK_NAME}: Average Utilization | acPMTrunkUtilizationAverage[{#SNMPINDEX}] | SNMP_AGENT |
| Trunk {#TRUNK_NAME}: Maximum Utilization | acPMTrunkUtilizationMax[{#SNMPINDEX}] | SNMP_AGENT |
| Trunk {#TRUNK_NAME}: Total Utilization | acPMTrunkUtilizationTotal[{#SNMPINDEX}] | SNMP_AGENT |
| Trunk {#TRUNK_NAME}: Deactivating alarms | acTrunkDeactivate[{#SNMPINDEX}] | SNMP_AGENT |
| Trunk {#TRUNK_NAME}: Alarm status | acTrunkStatusAlarm[{#SNMPINDEX}] | SNMP_AGENT |
| Trunk {#TRUNK_NAME}: D channel status | acTrunkStatusDChannel[{#SNMPINDEX}] | SNMP_AGENT |
