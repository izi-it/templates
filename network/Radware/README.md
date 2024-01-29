# SNMP Radware Alteon CPU
No template description
## Summary
* [discoveries](#discoveries)
  * [Discovery CPU ](#discovery_cpu
)
<a name="discoveries" />
## Discoveries

| name | key | type | delay |
| ------------- |------------- |------------- |------------- |
| CPU | spStatsCpuUtilSpIndex | SNMP_AGENT | 10 |

<a name="discovery_cpu" />
## Discovery CPU

### Items

| name | key | type |
| ------------- |------------- |------------- |
| Utilization of processor (1s) $1 $2 | spStatsCpuUtil1Seconds[{#CORE}] | SNMP_AGENT |
| Utilization of processor (4s) $1 $2 | spStatsCpuUtil4Seconds[{#CORE}] | SNMP_AGENT |
| Utilization of processor (64s) $1 $2 | spStatsCpuUtil64Seconds[{#CORE}] | SNMP_AGENT |

### Triggers

| name | expression | priority |
| ------------- |------------- |------------- |
| Average CPU usage | last(/SNMP Radware Alteon CPU/spStatsCpuUtil4Seconds[{#CORE}])>75 | AVERAGE |
| High CPU usage | last(/SNMP Radware Alteon CPU/spStatsCpuUtil4Seconds[{#CORE}])>=90 | HIGH |
