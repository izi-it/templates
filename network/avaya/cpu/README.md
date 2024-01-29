# SNMP Avaya cpu
Template to check Checkpoint cpu equipments using SNMP protocol by izi-it
## Summary
* [macros](#macros)
* [discoveries](#discoveries)
  * [Discovery Avaya cpu ](#discovery_avaya_cpu
)
<a name="macros" />
## Macros

| macro | value |
| ------------- |------------- |
| {$_CRITCPU} | 90 |
| {$_WARNCPU} | 80 |

<a name="discoveries" />
## Discoveries

| name | key | type | delay |
| ------------- |------------- |------------- |------------- |
| Avaya cpu | s5ChasUtilEntry-[{#SNMPVALUE}] | SNMP_AGENT | 1m |

<a name="discovery_avaya_cpu" />
## Discovery Avaya cpu

### Items

| name | key | type |
| ------------- |------------- |------------- |
| CPU {#SNMPINDEX}: Used CPU | s5ChasUtilTotalCPUUsage[{#SNMPINDEX}] | SNMP_AGENT |

### Triggers

| name | expression | priority |
| ------------- |------------- |------------- |
| CPU is above critical threshold | min(/SNMP Avaya cpu/s5ChasUtilTotalCPUUsage[{#SNMPINDEX}],5m)>{$_CRITCPU} | AVERAGE |
| CPU is above warning threshold | min(/SNMP Avaya cpu/s5ChasUtilTotalCPUUsage[{#SNMPINDEX}],5m)>{$_WARNCPU}<br>and<br>min(/SNMP Avaya cpu/s5ChasUtilTotalCPUUsage[{#SNMPINDEX}],5m)<{$_CRITCPU} | WARNING |
