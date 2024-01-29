# SNMP Fortinet VPN
Template to check Fortinet Fortigate equipments using SNMP protocol by izi-it
## Summary
* [macros](#macros)
* [discoveries](#discoveries)
  * [Discovery Fortinet vpn ](#discovery_fortinet_vpn
)
<a name="macros" />
## Macros

| macro | value |
| ------------- |------------- |
| {$_VPNEXCLUDE} | VPN-SPIE |

<a name="discoveries" />
## Discoveries

| name | key | type | delay |
| ------------- |------------- |------------- |------------- |
| Fortinet vpn | fgVpnTunEntPhase2Name-[{#SNMPVALUE}] | SNMP_AGENT | 1h |

<a name="discovery_fortinet_vpn" />
## Discovery Fortinet vpn

### Items

| name | key | type |
| ------------- |------------- |------------- |
| VPN {#PHASE2NAME}: Status | fgVpnTunEntStatus[{#SNMPINDEX}] | SNMP_AGENT |

### Triggers

| name | expression | priority |
| ------------- |------------- |------------- |
| VPN Status is down | last(/SNMP Fortinet VPN/fgVpnTunEntStatus[{#SNMPINDEX}])<>2 | HIGH |
