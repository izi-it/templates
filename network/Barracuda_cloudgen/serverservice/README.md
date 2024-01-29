# SNMP Barracuda cloudgen serverservice
Template to check SNMP Barracuda cloudgen equipments using SNMP protocol by izi-it
## Summary
* [discoveries](#discoveries)
  * [Discovery Barracuda cloudgen serverservice ](#discovery_barracuda_cloudgen_serverservice
)
<a name="discoveries" />
## Discoveries

| name | key | type | delay |
| ------------- |------------- |------------- |------------- |
| Barracuda cloudgen serverservice | serverServiceName-[{#SNMPVALUE}] | SNMP_AGENT | 1h |

<a name="discovery_barracuda_cloudgen_serverservice" />
## Discovery Barracuda cloudgen serverservice

### Items

| name | key | type |
| ------------- |------------- |------------- |
| Server Service {#SERVERSERVICE_NAME}: Status | serverServiceState[{#SNMPINDEX}] | SNMP_AGENT |
