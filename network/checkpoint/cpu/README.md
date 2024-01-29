# SNMP Checkpoint cpu
Template to check Checkpoint cpu equipments using SNMP protocol by izi-it
## Summary
* [items](#items)
* [triggers](#triggers)
* [discoveries](#discoveries)
  * [Discovery Checkpoint cpu ](#discovery_checkpoint_cpu
)
<a name="items" />
## Items

| name | key | type |
| ------------- |------------- |------------- |
| Overall CPU utilization | procUsage | SNMP_AGENT |

<a name="triggers" />
## Triggers

| name | expression | priority |
| ------------- |------------- |------------- |
| CPU utilization is above critical threshold | min(/SNMP Checkpoint cpu/procUsage,5m)>{$_CRITCPU} | HIGH |

<a name="discoveries" />
## Discoveries

| name | key | type | delay |
| ------------- |------------- |------------- |------------- |
| Checkpoint cpu | cpuusage-[{#SNMPVALUE}] | SNMP_AGENT | 1m |

<a name="discovery_checkpoint_cpu" />
## Discovery Checkpoint cpu

### Items

| name | key | type |
| ------------- |------------- |------------- |
| CPU {#CPU} Usage | cpuusage[{#SNMPINDEX}] | SNMP_AGENT |
