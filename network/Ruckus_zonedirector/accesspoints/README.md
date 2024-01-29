# SNMP Ruckus zonedirector accesspoints
Template SNMP Ruckus zonedirector accesspoints by automate@izi-it
Hash: xxxxxxxxxxxxxxx

Template to check Ruckus zonedirector equipments using SNMP protocol
## Summary
* [discoveries](#discoveries)
  * [Discovery Ruckus zonedirector accesspoints ](#discovery_ruckus_zonedirector_accesspoints
)
<a name="discoveries" />
## Discoveries

| name | key | type | delay |
| ------------- |------------- |------------- |------------- |
| Ruckus zonedirector accesspoints | ruckusZDWLANAPDescription-[{#SNMPVALUE}] | SNMP_AGENT | 5m |

<a name="discovery_ruckus_zonedirector_accesspoints" />
## Discovery Ruckus zonedirector accesspoints

### Items

| name | key | type |
| ------------- |------------- |------------- |
| AP {#AP_DESCRIPTION}: CPU utilization | ruckusZDWLANAPCPUUtil[{#SNMPINDEX}] | SNMP_AGENT |
| AP {#AP_DESCRIPTION}: Bytes received on LAN port | ruckusZDWLANAPLANStatsRXByte[{#SNMPINDEX}] | SNMP_AGENT |
| AP {#AP_DESCRIPTION}: Bytes transmitted on LAN port | ruckusZDWLANAPLANStatsTXByte[{#SNMPINDEX}] | SNMP_AGENT |
| AP {#AP_DESCRIPTION}: Total memory | ruckusZDWLANAPMemTotal[{#SNMPINDEX}] | SNMP_AGENT |
| AP {#AP_DESCRIPTION}: Memory utilization | ruckusZDWLANAPMemUtil[{#SNMPINDEX}] | SNMP_AGENT |
| AP {#AP_DESCRIPTION}: Number of rogue devices | ruckusZDWLANAPNumRogues[{#SNMPINDEX}] | SNMP_AGENT |
| AP {#AP_DESCRIPTION}: Total number of authenticated terminal | ruckusZDWLANAPNumSta[{#SNMPINDEX}] | SNMP_AGENT |
| AP {#AP_DESCRIPTION}: Number of APs | ruckusZDWLANAPNumVAP[{#SNMPINDEX}] | SNMP_AGENT |
| AP {#AP_DESCRIPTION}: Connection status with ZD | ruckusZDWLANAPStatus[{#SNMPINDEX}] | SNMP_AGENT |
