# SNMP Polycom rmx board
Template SNMP Polycom board  by automate@izi-it
Hash: xxxxxxxxxxxxxxx

Template to check Polycom rmx board equipments using SNMP protocol
## Summary
* [discoveries](#discoveries)
  * [Discovery Polycom rmx board ](#discovery_polycom_rmx_board
)
<a name="discoveries" />
## Discoveries

| name | key | type | delay |
| ------------- |------------- |------------- |------------- |
| Polycom rmx board | polycomhardwareboard-[{#SNMPVALUE}] | SNMP_AGENT | 1h |

<a name="discovery_polycom_rmx_board" />
## Discovery Polycom rmx board

### Items

| name | key | type |
| ------------- |------------- |------------- |
| BOARD {#BOARD}: Status | hardwareIntegratedBoardStatus[{#SNMPINDEX}] | SNMP_AGENT |
