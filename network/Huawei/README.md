# SNMP Huawei Switch S5700 Generic
No template description
## Summary
* [items](#items)
* [macros](#macros)
* [triggers](#triggers)

<a name="items" />
## Items

| name | key | type |
| ------------- |------------- |------------- |
| Number of network interfaces | HwifNumber | SNMP_AGENT |
| Switch configuration (stacked or standalone) | hwStackIsStackDevice | SNMP_AGENT |
| Ping Switch | icmpping | SIMPLE |

<a name="macros" />
## Macros

| macro | value |
| ------------- |------------- |
| {$PING_TIMEOUT_SWITCH} | NONE |

<a name="triggers" />
## Triggers

| name | expression | priority |
| ------------- |------------- |------------- |
| No contact with the switch for 3 minutes | max(/SNMP Huawei Switch S5700 Generic/icmpping,{$PING_TIMEOUT_SWITCH})=0 | DISASTER |
