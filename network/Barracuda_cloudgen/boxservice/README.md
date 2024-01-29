# SNMP Barracuda cloudgen boxservice
Template to check SNMP Barracuda cloudgen equipments using SNMP protocol by izi-it
## Summary
* [discoveries](#discoveries)
  * [Discovery Barracuda cloudgen boxservice ](#discovery_barracuda_cloudgen_boxservice
)
<a name="discoveries" />
## Discoveries

| name | key | type | delay |
| ------------- |------------- |------------- |------------- |
| Barracuda cloudgen boxservice | boxServiceName-[{#SNMPVALUE}] | SNMP_AGENT | 1h |

<a name="discovery_barracuda_cloudgen_boxservice" />
## Discovery Barracuda cloudgen boxservice

### Items

| name | key | type |
| ------------- |------------- |------------- |
| Boxservice {#BOXSERVICE_NAME}: Status | boxServiceState[{#SNMPINDEX}] | SNMP_AGENT |
