# SNMP Hirschmann classic fan
TemplateSNMP Hirschmann classic fan made by automate@izi-it
Hash: xxxxxxxxxxxxxxx
## Summary
* [discoveries](#discoveries)
  * [Discovery Hirschmann classic fan ](#discovery_hirschmann_classic_fan
)
<a name="discoveries" />
## Discoveries

| name | key | type | delay |
| ------------- |------------- |------------- |------------- |
| Hirschmann classic fan | hmFanID-[{#SNMPVALUE}] | SNMP_AGENT | 1m |

<a name="discovery_hirschmann_classic_fan" />
## Discovery Hirschmann classic fan

### Items

| name | key | type |
| ------------- |------------- |------------- |
| Fan {#FAN}: State | hmFanState[{#SNMPINDEX}] | SNMP_AGENT |
