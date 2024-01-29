# SNMP Efficientip dhcpusage
Template SNMP Efficientip dhcpusage  made by automate@izi-it
Hash: xxxxxxxxxxxxxxx
## Summary
* [discoveries](#discoveries)
  * [Discovery Efficientip dhcpusage ](#discovery_efficientip_dhcpusage
)
<a name="discoveries" />
## Discoveries

| name | key | type | delay |
| ------------- |------------- |------------- |------------- |
| Efficientip dhcpusage | eipDhcpStatName-[{#SNMPVALUE}] | SNMP_AGENT | 1m |

<a name="discovery_efficientip_dhcpusage" />
## Discovery Efficientip dhcpusage

### Items

| name | key | type |
| ------------- |------------- |------------- |
| DHCP {#DHCP_NAME}: Statistic value | eipDhcpStatValue[{#SNMPINDEX}] | SNMP_AGENT |
