# SNMP Huawei Switch S5700 Temperature
No template description
## Summary
* [macros](#macros)
* [discoveries](#discoveries)
  * [Discovery Discovery: Temperature ](#discovery_discovery:_temperature
)
<a name="macros" />
## Macros

| macro | value |
| ------------- |------------- |
| {$TEMP_CRIT} | 70 |
| {$TEMP_WARN} | 60 |

<a name="discoveries" />
## Discoveries

| name | key | type | delay |
| ------------- |------------- |------------- |------------- |
| Discovery: Temperature | hwEntityTemperature | SNMP_AGENT | 1h |

<a name="discovery_discovery:_temperature" />
## Discovery Discovery: Temperature

### Items

| name | key | type |
| ------------- |------------- |------------- |
| Unit-[$1] Temperature | hwEntityTemperature[{#SNMPINDEX}] | SNMP_AGENT |

### Triggers

| name | expression | priority |
| ------------- |------------- |------------- |
| Unit-[{#SNMPINDEX}] Temperature ALERT | min(/SNMP Huawei Switch S5700 Temperature/hwEntityTemperature[{#SNMPINDEX}],5m)>={$TEMP_CRIT} | HIGH |
| Unit-[{#SNMPINDEX}] Temperature WARNING | min(/SNMP Huawei Switch S5700 Temperature/hwEntityTemperature[{#SNMPINDEX}],5m)>={$TEMP_WARN} | WARNING |
