# SNMP Avaya memory
Template to check Checkpoint memory equipments using SNMP protocol by izi-it
## Summary
* [macros](#macros)
* [discoveries](#discoveries)
  * [Discovery Avaya memory ](#discovery_avaya_memory
)
<a name="macros" />
## Macros

| macro | value |
| ------------- |------------- |
| {$_CRITMEM} | 90 |
| {$_WARNMEM} | 80 |

<a name="discoveries" />
## Discoveries

| name | key | type | delay |
| ------------- |------------- |------------- |------------- |
| Avaya memory | s5ChasUtilMemory-[{#SNMPVALUE}] | SNMP_AGENT | 1m |

<a name="discovery_avaya_memory" />
## Discovery Avaya memory

### Items

| name | key | type |
| ------------- |------------- |------------- |
| Memory {#SNMPINDEX}: Available Memory | s5ChasUtilMemoryAvailable[{#SNMPINDEX}] | SNMP_AGENT |
| Memory {#SNMPINDEX}: Total Memory | s5ChasUtilMemoryTotal[{#SNMPINDEX}] | SNMP_AGENT |
| Memory {#SNMPINDEX}: Used Memory | s5ChasUtilMemoryUsed[{#SNMPINDEX}] | CALCULATED |

### Triggers

| name | expression | priority |
| ------------- |------------- |------------- |
| Used Memory is above critical threshold | min(/SNMP Avaya memory/s5ChasUtilMemoryUsed[{#SNMPINDEX}],5m)> {$_CRITMEM} | AVERAGE |
| Used Memory is above warning threshold | min(/SNMP Avaya memory/s5ChasUtilMemoryUsed[{#SNMPINDEX}],5m)>{$_WARNMEM}<br>and min(/SNMP Avaya memory/s5ChasUtilMemoryUsed[{#SNMPINDEX}],5m)<{$_CRITMEM} | WARNING |
