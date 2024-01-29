# SNMP Huawei Switch S5700 Stack Health
No template description
## Summary
* [discoveries](#discoveries)
  * [Discovery Stack Cable Connectivity [$1] ](#discovery_stack_cable_connectivity_[$1]
)
<a name="discoveries" />
## Discoveries

| name | key | type | delay |
| ------------- |------------- |------------- |------------- |
| Stack Cable Connectivity [$1] | hwStackPortStatus | SNMP_AGENT | 1h |

<a name="discovery_stack_cable_connectivity_[$1]" />
## Discovery Stack Cable Connectivity [$1]

### Items

| name | key | type |
| ------------- |------------- |------------- |
| Stack Cable Connectivity [$1] | hwStackPortStatus[{#SNMPINDEX}] | SNMP_AGENT |

### Triggers

| name | expression | priority |
| ------------- |------------- |------------- |
| Unit-[{#SNMPINDEX}] Stack link is DOWN | last(/SNMP Huawei Switch S5700 Stack Health/hwStackPortStatus[{#SNMPINDEX}])<>1 | DISASTER |
