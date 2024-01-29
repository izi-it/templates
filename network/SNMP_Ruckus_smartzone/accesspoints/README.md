# SNMP Ruckus smartzone accesspoints
Template SNMP Ruckus smartzone accesspoints by automate@izi-it
Hash: xxxxxxxxxxxxxxx

Template to check Ruckus smartzone equipments using SNMP protocol
## Summary
* [discoveries](#discoveries)
  * [Discovery Ruckus smartzone accesspoints ](#discovery_ruckus_smartzone_accesspoints
)
<a name="discoveries" />
## Discoveries

| name | key | type | delay |
| ------------- |------------- |------------- |------------- |
| Ruckus smartzone accesspoints | ruckusSZAPName-[{#SNMPVALUE}] | SNMP_AGENT | 5m |

<a name="discovery_ruckus_smartzone_accesspoints" />
## Discovery Ruckus smartzone accesspoints

### Items

| name | key | type |
| ------------- |------------- |------------- |
| AP {#AP_NAME}: Configuration Status | ruckusSZAPConfigStatus[{#SNMPINDEX}] | SNMP_AGENT |
| AP {#AP_NAME}: Current connection status | ruckusSZAPConnStatus[{#SNMPINDEX}] | SNMP_AGENT |
| AP {#AP_NAME}: Number of bytes received in IPsec session | ruckusSZAPIpsecRXBytes[{#SNMPINDEX}] | SNMP_AGENT |
| AP {#AP_NAME}: Number of bytes transmitted in IPsec session | ruckusSZAPIpsecTXBytes[{#SNMPINDEX}] | SNMP_AGENT |
| AP {#AP_NAME}: Model | ruckusSZAPModel[{#SNMPINDEX}] | SNMP_AGENT |
| AP {#AP_NAME}: Number of concurrently connected clients | ruckusSZAPNumSta[{#SNMPINDEX}] | SNMP_AGENT |
| AP {#AP_NAME}: Current registration status | ruckusSZAPRegStatus[{#SNMPINDEX}] | SNMP_AGENT |
| AP {#AP_NAME}: Serial number | ruckusSZAPSerial[{#SNMPINDEX}] | SNMP_AGENT |
