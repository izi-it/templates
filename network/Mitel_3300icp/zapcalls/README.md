# SNMP Mitel 3300icp zapcalls
Template SNMP Mitel 3300icp zapcalls by automate@izi-it
Hash: xxxxxxxxxxxxxxx

Template to check SNMP Mitel 3300icp equipments using SNMP protocol
## Summary
* [discoveries](#discoveries)
  * [Discovery Mitel 3300icp zapcalls ](#discovery_mitel_3300icp_zapcalls
)
<a name="discoveries" />
## Discoveries

| name | key | type | delay |
| ------------- |------------- |------------- |------------- |
| Mitel 3300icp zapcalls | mitelBWMCurrentZAPLabel-[{#SNMPVALUE}] | SNMP_AGENT | 5m |

<a name="discovery_mitel_3300icp_zapcalls" />
## Discovery Mitel 3300icp zapcalls

### Items

| name | key | type |
| ------------- |------------- |------------- |
| Zone Access Point Label {#ZAP_LABEL}: Number of calls admitted | mitelBWMCumCACAdmissions[{#SNMPINDEX}] | SNMP_AGENT |
| Zone Access Point Label {#ZAP_LABEL}: Rejected calls ratio | mitelBWMCumCACRejectionRatio[{#SNMPINDEX}] | SNMP_AGENT |
| Zone Access Point Label {#ZAP_LABEL}: Number of calls rejected | mitelBWMCumCACRejections[{#SNMPINDEX}] | SNMP_AGENT |
