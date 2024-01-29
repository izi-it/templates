# SNMP Citrix netscaler vserverstatus
No template description
## Summary
* [items](#items)
* [discoveries](#discoveries)
  * [Discovery Netscaler vserverstatus ](#discovery_netscaler_vserverstatus
)
<a name="items" />
## Items

| name | key | type |
| ------------- |------------- |------------- |
| Number of CPUs | numCPUs | SNMP_AGENT |

<a name="discoveries" />
## Discoveries

| name | key | type | delay |
| ------------- |------------- |------------- |------------- |
| Netscaler vserverstatus | vsvrFullName-[{#SNMPVALUE}] | SNMP_AGENT | 1m |

<a name="discovery_netscaler_vserverstatus" />
## Discovery Netscaler vserverstatus

### Items

| name | key | type |
| ------------- |------------- |------------- |
| Vsrv  {#VSRV} Type | vsvrEntityType[{#SNMPINDEX}] | SNMP_AGENT |
| Vsrv  {#VSRV} Ip Address | vsvrIpAddress[{#SNMPINDEX}] | SNMP_AGENT |
| Vsrv  {#VSRV} Port | vsvrPort[{#SNMPINDEX}] | SNMP_AGENT |
| Vsrv  {#VSRV} Status | vsvrState[{#SNMPINDEX}] | SNMP_AGENT |
| Vsrv  {#VSRV}  number Surge queue | vsvrSurgeCount[{#SNMPINDEX}] | SNMP_AGENT |
| Vsrv  {#VSRV} Total Clients | vsvrTotalClients[{#SNMPINDEX}] | SNMP_AGENT |
| Vsrv  {#VSRV} Total Requests Bytes | vsvrTotalRequestBytes[{#SNMPINDEX}] | SNMP_AGENT |
| Vsrv  {#VSRV} Total Requests | vsvrTotalRequests[{#SNMPINDEX}] | SNMP_AGENT |
| Vsrv  {#VSRV} Total Responses Bytes | vsvrTotalResponseBytes[{#SNMPINDEX}] | SNMP_AGENT |
| Vsrv  {#VSRV} Total Responses | vsvrTotalResponses[{#SNMPINDEX}] | SNMP_AGENT |
