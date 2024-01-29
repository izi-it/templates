# SNMP Citrix sdx hardware
Template SNMP Citrix srx hardware by automate@izi-it
Hash: xxxxxxxxxxxxxxx

Check hardware.
## Summary
* [discoveries](#discoveries)
  * [Discovery Citrix sdx hardwareResourceName ](#discovery_citrix_sdx_hardwareresourcename
)  * [Discovery Citrix sdx softwareResourceName ](#discovery_citrix_sdx_softwareresourcename
)
<a name="discoveries" />
## Discoveries

| name | key | type | delay |
| ------------- |------------- |------------- |------------- |
| Citrix sdx hardwareResourceName | hardwareResourceName-[{#SNMPVALUE}] | SNMP_AGENT | 5m |
| Citrix sdx softwareResourceName | softwareResourceName-[{#SNMPVALUE}] | SNMP_AGENT | 5m |

<a name="discovery_citrix_sdx_hardwareresourcename" />
## Discovery Citrix sdx hardwareResourceName

### Items

| name | key | type |
| ------------- |------------- |------------- |
| Hardware Resource {#HARDWARE_RESOURCENAME}: Health status | hardwareResourceStatus[{#SNMPINDEX}] | SNMP_AGENT |

<a name="discovery_citrix_sdx_softwareresourcename" />
## Discovery Citrix sdx softwareResourceName

### Items

| name | key | type |
| ------------- |------------- |------------- |
| Software Resource {#SOFTWARE_RESOURCENAME}: Health status | softwareResourceStatus[{#SNMPINDEX}] | SNMP_AGENT |
