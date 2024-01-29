# SNMP Mcafee webgateway cpu
Template to check SNMP Mcafee webgateway cpu equipments using SNMP protocol by izi-it
## Summary
* [macros](#macros)
* [discoveries](#discoveries)
  * [Discovery Mcafee cpu ](#discovery_mcafee_cpu
)
<a name="macros" />
## Macros

| macro | value |
| ------------- |------------- |
| {$LISTPROCESSUS} | mwg-core |

<a name="discoveries" />
## Discoveries

| name | key | type | delay |
| ------------- |------------- |------------- |------------- |
| Mcafee cpu | stCPULoad-[{#SNMPVALUE}] | SNMP_AGENT | 5m |

<a name="discovery_mcafee_cpu" />
## Discovery Mcafee cpu

### Items

| name | key | type |
| ------------- |------------- |------------- |
| CPU Process {#PROCESSCPU}: Utilization | mcafeecpuload[{#SNMPINDEX}] | SNMP_AGENT |

### Triggers

| name | expression | priority |
| ------------- |------------- |------------- |
| CPU Process {$_PROCESS} is above critical threshold | last(/SNMP Mcafee webgateway cpu/mcafeecpuload[{#SNMPINDEX}])> {$_CPU_CRIT} | HIGH |
| CPU Process {$_PROCESS} is above warning  threshold | last(/SNMP Mcafee webgateway cpu/mcafeecpuload[{#SNMPINDEX}])> {$_CPU_WARN}<br>and <br>last(/SNMP Mcafee webgateway cpu/mcafeecpuload[{#SNMPINDEX}])< {$_CPU_CRIT} | WARNING |
