# SNMP A10 AX vserverusage
Template SNMP A10 AX vserverusage made by automate@izi-it
Hash: xxxxxxxxxxxxxxx

Check virtual server usage.
## Summary
* [discoveries](#discoveries)
  * [Discovery A10 AX vserverusage ](#discovery_a10_ax_vserverusage
)
<a name="discoveries" />
## Discoveries

| name | key | type | delay |
| ------------- |------------- |------------- |------------- |
| A10 AX vserverusage | axVirtualServerName-[{#SNMPVALUE}] | SNMP_AGENT | 1m |

<a name="discovery_a10_ax_vserverusage" />
## Discovery A10 AX vserverusage

### Items

| name | key | type |
| ------------- |------------- |------------- |
| Virtual Server {#VIRTUALSERVER_NAME} : Number of bytes received from client to server | axVirtualServerStatBytesIn[{#SNMPINDEX}] | SNMP_AGENT |
| Virtual Server {#VIRTUALSERVER_NAME} : Number of bytes sent from server to client | axVirtualServerStatBytesOut[{#SNMPINDEX}] | SNMP_AGENT |
| Virtual Server {#VIRTUALSERVER_NAME} : Current connections from client side | axVirtualServerStatCurConns[{#SNMPINDEX}] | SNMP_AGENT |
| Virtual Server {#VIRTUALSERVER_NAME} : Current virtual server status | axVirtualServerStatStatus1[{#SNMPINDEX}] | SNMP_AGENT |
| Virtual Server {#VIRTUALSERVER_NAME} : Total connections from client side | axVirtualServerStatTotConns[{#SNMPINDEX}] | SNMP_AGENT |
