# SNMP Huawei Switch S5700 Memory
No template description
## Summary
* [discoveries](#discoveries)
  * [Discovery Discovery: Memory ](#discovery_discovery:_memory
)
<a name="discoveries" />
## Discoveries

| name | key | type | delay |
| ------------- |------------- |------------- |------------- |
| Discovery: Memory | hwMemoryDev | SNMP_AGENT | 1h |

<a name="discovery_discovery:_memory" />
## Discovery Discovery: Memory

### Items

| name | key | type |
| ------------- |------------- |------------- |
| Unit-[$1] Memory allocation failures due to no idle memory | hwMemoryDevFailNoMem[{#SNMPINDEX}] | SNMP_AGENT |
| Unit-[$1] Memory allocation failure count | hwMemoryDevFail[{#SNMPINDEX}] | SNMP_AGENT |
| Unit-[$1] Memory Free | hwMemoryDevFree[{#SNMPINDEX}] | SNMP_AGENT |
| Unit-[$1] Memory Used | hwMemoryDevRawSliceUsed[{#SNMPINDEX}] | SNMP_AGENT |
| Unit-[$1] Memory Total Size | hwMemoryDevSize[{#SNMPINDEX}] | SNMP_AGENT |
| Unit-[{#SNMPINDEX}] Memory Free (%) | memFreePercentage[{#SNMPINDEX}] | CALCULATED |
| Unit-[{#SNMPINDEX}] Memory Used (%) | memUsedPercentage[{#SNMPINDEX}] | CALCULATED |

### Triggers

| name | expression | priority |
| ------------- |------------- |------------- |
| Unit-[{#SNMPINDEX}] Available memory was below 5% for 5min | min(/SNMP Huawei Switch S5700 Memory/memFreePercentage[{#SNMPINDEX}],5m)<=5 | HIGH |
| Unit-[{#SNMPINDEX}] Available memory was below 10% for 5min | min(/SNMP Huawei Switch S5700 Memory/memFreePercentage[{#SNMPINDEX}],5m)<=10 | WARNING |
| Unit-[{#SNMPINDEX}] Memory usage is above 90% for 5min | min(/SNMP Huawei Switch S5700 Memory/memUsedPercentage[{#SNMPINDEX}],5m)>=90 | WARNING |
| Unit-[{#SNMPINDEX}] Memory usage is above 95% for 5min | min(/SNMP Huawei Switch S5700 Memory/memUsedPercentage[{#SNMPINDEX}],5m)>=95 | HIGH |
