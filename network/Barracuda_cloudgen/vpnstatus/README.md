# SNMP Barracuda cloudgen vpnstatus
Template to check SNMP Barracuda cloudgen equipments using SNMP protocol by izi-it
## Summary
* [discoveries](#discoveries)
  * [Discovery Barracuda cloudgen vpnstatus ](#discovery_barracuda_cloudgen_vpnstatus
)
<a name="discoveries" />
## Discoveries

| name | key | type | delay |
| ------------- |------------- |------------- |------------- |
| Barracuda cloudgen vpnstatus | vpnName-[{#SNMPVALUE}] | SNMP_AGENT | 1h |

<a name="discovery_barracuda_cloudgen_vpnstatus" />
## Discovery Barracuda cloudgen vpnstatus

### Items

| name | key | type |
| ------------- |------------- |------------- |
| VPN {#VPN_NAME}: Status | vpnState[{#SNMPINDEX}] | SNMP_AGENT |
