# SNMP Denyall listreverseproxy
Template SNMP Denyall listreverseproxy made by automate@izi-it
Hash: xxxxxxxxxxxxxxx

List reverse proxies.
## Summary
* [discoveries](#discoveries)
  * [Discovery Denyall listreverseproxy ](#discovery_denyall_listreverseproxy
)
<a name="discoveries" />
## Discoveries

| name | key | type | delay |
| ------------- |------------- |------------- |------------- |
| Denyall listreverseproxy | uid-[{#SNMPVALUE}] | SNMP_AGENT | 1m |

<a name="discovery_denyall_listreverseproxy" />
## Discovery Denyall listreverseproxy

### Items

| name | key | type |
| ------------- |------------- |------------- |
| Reverse Proxy {#REVERSEPROXY_UID}: CPU Usage | rpCpuUsage[{#SNMPINDEX}] | SNMP_AGENT |
| Reverse Proxy {#REVERSEPROXY_UID}: Memory Usage | rpMemoryUsage[{#SNMPINDEX}] | SNMP_AGENT |
| Reverse Proxy {#REVERSEPROXY_UID}: Requests psec | rpRqstsPrSecond[{#SNMPINDEX}] | SNMP_AGENT |
| Reverse Proxy {#REVERSEPROXY_UID}: Status | rpStatus[{#SNMPINDEX}] | SNMP_AGENT |
