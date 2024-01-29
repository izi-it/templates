# SNMP Infoblox services
Template SNMP Infoblox services made by automate@izi-it
Hash: xxxxxxxxxxxxxxx
## Summary
* [discoveries](#discoveries)
  * [Discovery Infoblox services ](#discovery_infoblox_services
)
<a name="discoveries" />
## Discoveries

| name | key | type | delay |
| ------------- |------------- |------------- |------------- |
| Infoblox services | ibNodeServiceName-[{#SNMPVALUE}] | SNMP_AGENT | 1m |

<a name="discovery_infoblox_services" />
## Discovery Infoblox services

### Items

| name | key | type |
| ------------- |------------- |------------- |
| Service {#SERVICE_NAME}: State | ibNodeServiceStatus[{#SNMPINDEX}] | SNMP_AGENT |
