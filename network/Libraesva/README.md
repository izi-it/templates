# SNMP Libraesva
No template description
## Summary
* [items](#items)
* [triggers](#triggers)

<a name="items" />
## Items

| name | key | type |
| ------------- |------------- |------------- |
| Cluster Status | clusterStatus | SNMP_AGENT |
| Mails queue in | incomingMailQueue | SNMP_AGENT |
| Mail Bounced | mailBounced | SNMP_AGENT |
| Mail Received | mailReceived | SNMP_AGENT |
| Mail Rejected | mailRejected | SNMP_AGENT |
| Mail Sent | mailSent | SNMP_AGENT |
| SMTP service | net.tcp.service.perf[smtp] | SIMPLE |
| HTTPS service | net.tcp.service[https] | SIMPLE |
| SSH service | net.tcp.service[ssh] | SIMPLE |
| Mails queue out | outgoingMailQueue | SNMP_AGENT |
| ESVA Version | prodVersion | SNMP_AGENT |
| Mails queue in Delta | queueInDelta | CALCULATED |
| Mails queue out Delta | queueOutDelta | CALCULATED |
| Mail Spam | spamMessages | SNMP_AGENT |
| Mail virus | virusMessages | SNMP_AGENT |

<a name="triggers" />
## Triggers

| name | expression | priority |
| ------------- |------------- |------------- |
| Cluster Error on {HOST.NAME} | min(/SNMP Libraesva/clusterStatus,#5)>0 | HIGH |
| Queue IN on {HOST.NAME} | min(/SNMP Libraesva/incomingMailQueue,30m)>100 and min(/SNMP Libraesva/incomingMailQueue,30m)>4*avg(/SNMP Libraesva/incomingMailQueue,7d)  and forecast(/SNMP Libraesva/incomingMailQueue,1200s,3600s)>100 | HIGH |
| SMTP on {HOST.NAME} | max(/SNMP Libraesva/net.tcp.service.perf[smtp],3m)=0 | WARNING |
| HTTP on {HOST.NAME} | max(/SNMP Libraesva/net.tcp.service[https],3m)=0 | WARNING |
| SSH service ACTIVE on {HOST.NAME} | max(/SNMP Libraesva/net.tcp.service[ssh],1m)=1 | WARNING |
| Queue OUT on {HOST.NAME} | min(/SNMP Libraesva/outgoingMailQueue,30m)>200 and min(/SNMP Libraesva/outgoingMailQueue,30m)>6*avg(/SNMP Libraesva/outgoingMailQueue,7d) | HIGH |
