# SNMP Beeware reverseproxyusage
Template SNMP Beeware reverseproxyusage by automate@izi-it
Hash: xxxxxxxxxxxxxxx

Template to check Beeware equipments using SNMP protocol
## Summary
* [discoveries](#discoveries)
  * [Discovery Beeware reverseproxyusage ](#discovery_beeware_reverseproxyusage
)
<a name="discoveries" />
## Discoveries

| name | key | type | delay |
| ------------- |------------- |------------- |------------- |
| Beeware reverseproxyusage | beewarerp-[{#SNMPVALUE}] | SNMP_AGENT | 5m |

<a name="discovery_beeware_reverseproxyusage" />
## Discovery Beeware reverseproxyusage

### Items

| name | key | type |
| ------------- |------------- |------------- |
| Reverse Proxy {#RP_NAME}: CPU Utilization | beewarecpu[{#SNMPINDEX}] | SNMP_AGENT |
| Reverse Proxy {#RP_NAME}: Memory Used | beewarememory[{#SNMPINDEX}] | SNMP_AGENT |
| Reverse Proxy {#RP_NAME}: NB chils | beewarenbchils[{#SNMPINDEX}] | SNMP_AGENT |
| Reverse Proxy {#RP_NAME}: Status | beewarerunning[{#SNMPINDEX}] | SNMP_AGENT |
