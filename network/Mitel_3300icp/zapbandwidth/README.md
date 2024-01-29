# SNMP Mitel 3300icp zapbandwidth
Template SNMP Mitel 3300icp zapbandwidth by automate@izi-it
Hash: xxxxxxxxxxxxxxx

Template to check SNMP Mitel 3300icp equipments using SNMP protocol
## Summary
* [discoveries](#discoveries)
  * [Discovery Mitel 3300icp zapbandwidth ](#discovery_mitel_3300icp_zapbandwidth
)
<a name="discoveries" />
## Discoveries

| name | key | type | delay |
| ------------- |------------- |------------- |------------- |
| Mitel 3300icp zapbandwidth | mitelBWMCurrentZAPLabel-[{#SNMPVALUE}] | SNMP_AGENT | 5m |

<a name="discovery_mitel_3300icp_zapbandwidth" />
## Discovery Mitel 3300icp zapbandwidth

### Items

| name | key | type |
| ------------- |------------- |------------- |
| Zone Access Point Label {#ZAP_LABEL}: Bandwidth currently in use | mitelBWMCurrentBandwidthInUse[{#SNMPINDEX}] | SNMP_AGENT |
| Zone Access Point Label {#ZAP_LABEL}: Limit Bandwidth | mitelBWMCurrentBandwidthLimit[{#SNMPINDEX}] | SNMP_AGENT |
