# SNMP Huawei Switch S5700 CPU
No template description
## Summary
* [discoveries](#discoveries)
  * [Discovery Discovery : CPU Usage ](#discovery_discovery_:_cpu_usage
)
<a name="discoveries" />
## Discoveries

| name | key | type | delay |
| ------------- |------------- |------------- |------------- |
| Discovery : CPU Usage | hwAvgDuty | SNMP_AGENT | 1h |

<a name="discovery_discovery_:_cpu_usage" />
## Discovery Discovery : CPU Usage

### Items

| name | key | type |
| ------------- |------------- |------------- |
| Unit-[$1] CPU Usage in 1 min | hwAvgDuty1min[{#SNMPINDEX}] | SNMP_AGENT |
| Unit-[$1] CPU Usage in 5 min | hwAvgDuty5min[{#SNMPINDEX}] | SNMP_AGENT |

### Triggers

| name | expression | priority |
| ------------- |------------- |------------- |
| Unit-[{#SNMPINDEX}] CPU usage is above 60% for 5min | min(/SNMP Huawei Switch S5700 CPU/hwAvgDuty5min[{#SNMPINDEX}],5s)>=60 | AVERAGE |
| Unit-[{#SNMPINDEX}] CPU usage is above 80% for 5min | min(/SNMP Huawei Switch S5700 CPU/hwAvgDuty5min[{#SNMPINDEX}],5s)>=80 | HIGH |
