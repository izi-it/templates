# SNMP Citrix sdx xenusage
Template SNMP Citrix srx xenusage by automate@izi-it
Hash: xxxxxxxxxxxxxxx

Check xen hypervisors.
## Summary
* [discoveries](#discoveries)
  * [Discovery Citrix sdx xenusage ](#discovery_citrix_sdx_xenusage
)
<a name="discoveries" />
## Discoveries

| name | key | type | delay |
| ------------- |------------- |------------- |------------- |
| Citrix sdx xenusage | xenHostname-[{#SNMPVALUE}] | SNMP_AGENT | 5m |

<a name="discovery_citrix_sdx_xenusage" />
## Discovery Citrix sdx xenusage

### Items

| name | key | type |
| ------------- |------------- |------------- |
| Xen hypervisors {#XEN_HOSTNAME}: CPU Usage | xenCpuUsage[{#SNMPINDEX}] | SNMP_AGENT |
| Xen hypervisors {#XEN_HOSTNAME}: Free memory | xenMemoryFree[{#SNMPINDEX}] | SNMP_AGENT |
| Xen hypervisors {#XEN_HOSTNAME}: Total memory | xenMemoryTotal[{#SNMPINDEX}] | SNMP_AGENT |
