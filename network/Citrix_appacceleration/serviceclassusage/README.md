# SNMP Citrix appacceleration serviceclassusage
Template SNMP Citrix appacceleration serviceclassusage by automate@izi-it
Hash: xxxxxxxxxxxxxxx

Check service class usage.
## Summary
* [discoveries](#discoveries)
  * [Discovery Citrix appacceleration serviceclassusage ](#discovery_citrix_appacceleration_serviceclassusage
)
<a name="discoveries" />
## Discoveries

| name | key | type | delay |
| ------------- |------------- |------------- |------------- |
| Citrix appacceleration serviceclassusage | wsServiceClassName-[{#SNMPVALUE}] | SNMP_AGENT | 5m |

<a name="discovery_citrix_appacceleration_serviceclassusage" />
## Discovery Citrix appacceleration serviceclassusage

### Items

| name | key | type |
| ------------- |------------- |------------- |
| Service class {#SERVICE_CLASSNAME}: Number of accelerated octets received | wsScsCompressReceivedOctets[{#SNMPINDEX}] | SNMP_AGENT |
| Service class {#SERVICE_CLASSNAME}: Number of accelerated octets sent | wsScsCompressSentOctets[{#SNMPINDEX}] | SNMP_AGENT |
| Service class {#SERVICE_CLASSNAME}: Current number of accelerated connections | wsScsCurrentAcceleratedConnections[{#SNMPINDEX}] | SNMP_AGENT |
| Service class {#SERVICE_CLASSNAME}: Number of accelerated octets received before compression | wsScsPreCompressReceivedOctets[{#SNMPINDEX}] | SNMP_AGENT |
| Service class {#SERVICE_CLASSNAME}: Number of accelerated octets sent before compression | wsScsPreCompressSentOctets[{#SNMPINDEX}] | SNMP_AGENT |
| Service class {#SERVICE_CLASSNAME}: Total number of accelerated connections | wsScsTotalAcceleratedConnections[{#SNMPINDEX}] | SNMP_AGENT |
| Service class {#SERVICE_CLASSNAME}: Total number of non-accelerated connections | wsScsTotalNonAcceleratedConnections[{#SNMPINDEX}] | SNMP_AGENT |
