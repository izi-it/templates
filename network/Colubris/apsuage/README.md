# SNMP Colubris  apsuage
Template SNMP Colubris  apsuage by automate@izi-it
Hash: xxxxxxxxxxxxxxx

Check AP status and users connected.
## Summary
* [discoveries](#discoveries)
  * [Discovery Colubris  apsuage ](#discovery_colubris__apsuage
)
<a name="discoveries" />
## Discoveries

| name | key | type | delay |
| ------------- |------------- |------------- |------------- |
| Colubris  apsuage | coDevDisControllerIndex-[{#SNMPVALUE}] | SNMP_AGENT | 5m |

<a name="discovery_colubris__apsuage" />
## Discovery Colubris  apsuage

### Items

| name | key | type |
| ------------- |------------- |------------- |
| Controller index {#CONTROLLER_INDEX}: Device state | coDevDisState[{#SNMPINDEX}] | SNMP_AGENT |
| Controller index {#CONTROLLER_INDEX}: Device name | wsScsCurrentAcceleratedConnections[{#SNMPINDEX}] | SNMP_AGENT |
