# SNMP Stonesoft clusterstate
Template SNMP Stonesoft by automate@izi-it
Hash: xxxxxxxxxxxxxxx

Template to check SNMP Stonesoft clusterstate equipments using SNMP protocol
## Summary
* [discoveries](#discoveries)
  * [Discovery Stonesoft clusterstate ](#discovery_stonesoft_clusterstate
)
<a name="discoveries" />
## Discoveries

| name | key | type | delay |
| ------------- |------------- |------------- |------------- |
| Stonesoft clusterstate | nodeMemberId-[{#SNMPVALUE}] | SNMP_AGENT | 5m |

<a name="discovery_stonesoft_clusterstate" />
## Discovery Stonesoft clusterstate

### Items

| name | key | type |
| ------------- |------------- |------------- |
| Cluster Node {#NODEMEMBER_ID}: Status | nodeOperState[{#SNMPINDEX}] | SNMP_AGENT |
