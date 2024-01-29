# SNMP Microsens G6 hardware
Template SNMP Microsens G6 hardware made by automate@izi-it
Hash: xxxxxxxxxxxxxxx

.
## Summary
* [items](#items)
* [triggers](#triggers)

<a name="items" />
## Items

| name | key | type |
| ------------- |------------- |------------- |
| Fan State | hardwareFanStatus | SNMP_AGENT |
| PSU 1 State | hardwarePowerSupply1Status | SNMP_AGENT |
| PSU 2 State | hardwarePowerSupply2Status | SNMP_AGENT |
| Sd-Card State | hardwareSdCardStatus | SNMP_AGENT |
| Temperature value | systemTemperature | SNMP_AGENT |

<a name="triggers" />
## Triggers

| name | expression | priority |
| ------------- |------------- |------------- |
| Fan state is degraded | count(/SNMP Microsens G6 hardware/hardwareFanStatus,#3)=2 | WARNING |
