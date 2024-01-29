# SNMP Mcafee webgateway sessions
Template to check SNMP Mcafee webgateway sessions equipments using SNMP protocol by izi-it
## Summary
* [items](#items)
* [triggers](#triggers)

<a name="items" />
## Items

| name | key | type |
| ------------- |------------- |------------- |
| Number of active TCP sessions | mcafeetcpactivesessions | SNMP_AGENT |

<a name="triggers" />
## Triggers

| name | expression | priority |
| ------------- |------------- |------------- |
| Number of active TCP sessions is above critical threshold | last(/SNMP Mcafee webgateway sessions/mcafeetcpactivesessions)> {$_SESSION_CRIT} | HIGH |
