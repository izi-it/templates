# SNMP Huawei Switch S5700 Fan
No template description
## Summary
* [discoveries](#discoveries)
  * [Discovery Discovery: Fan ](#discovery_discovery:_fan
)
<a name="discoveries" />
## Discoveries

| name | key | type | delay |
| ------------- |------------- |------------- |------------- |
| Discovery: Fan | hwEntityFan | SNMP_AGENT | 1h |

<a name="discovery_discovery:_fan" />
## Discovery Discovery: Fan

### Items

| name | key | type |
| ------------- |------------- |------------- |
| Fan module [{#SNMPINDEX}] speed (%) | hwEntityFanSpeed[{#SNMPINDEX}] | SNMP_AGENT |
| Fan module [{#SNMPINDEX}] state | hwEntityFanState[{#SNMPINDEX}] | SNMP_AGENT |

### Triggers

| name | expression | priority |
| ------------- |------------- |------------- |
| Fan module [{#SNMPINDEX}] speed is above 60% (Possible high temperature!) | min(/SNMP Huawei Switch S5700 Fan/hwEntityFanSpeed[{#SNMPINDEX}],5m)>={$TEMP_WARN} and min(/SNMP Huawei Switch S5700 Fan/hwEntityFanSpeed[{#SNMPINDEX}],5m)<{$TEMP_CRIT} | WARNING |
| Fan module [{#SNMPINDEX}] speed is above 70% (Possible high temperature!) | min(/SNMP Huawei Switch S5700 Fan/hwEntityFanSpeed[{#SNMPINDEX}],5m)>={$TEMP_CRIT} | HIGH |
| Fan module [{#SNMPINDEX}] state is ABNORMAL | last(/SNMP Huawei Switch S5700 Fan/hwEntityFanState[{#SNMPINDEX}],#1)<>1 | WARNING |
