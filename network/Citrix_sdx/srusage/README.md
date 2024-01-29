# SNMP Citrix sdx srusage
Template SNMP Citrix srx srusage by automate@izi-it
Hash: xxxxxxxxxxxxxxx

Check storage repositories.
## Summary
* [discoveries](#discoveries)
  * [Discovery Citrix sdx srusage ](#discovery_citrix_sdx_srusage
)
<a name="discoveries" />
## Discoveries

| name | key | type | delay |
| ------------- |------------- |------------- |------------- |
| Citrix sdx srusage | srName-[{#SNMPVALUE}] | SNMP_AGENT | 5m |

<a name="discovery_citrix_sdx_srusage" />
## Discovery Citrix sdx srusage

### Items

| name | key | type |
| ------------- |------------- |------------- |
| Storage repository {#SR_NAME}: Size | srSize[{#SNMPINDEX}] | SNMP_AGENT |
| Storage repository {#SR_NAME}: Status | srStatus[{#SNMPINDEX}] | SNMP_AGENT |
| Storage repository {#SR_NAME}: Utilization | srUtilized[{#SNMPINDEX}] | SNMP_AGENT |
