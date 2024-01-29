# SNMP Ruckus SmartCell Gateway
Template SNMP Ruckus SCG by automate@izi-it
Hash: xxxxxxxxxxxxxxx

Template to check Ruckus SCG equipments using SNMP protocol
## Summary
* [items](#items)
* [discoveries](#discoveries)
  * [Discovery Ruckus APs ](#discovery_ruckus_aps
)  * [Discovery Ruckus SSIDs ](#discovery_ruckus_ssids
)
<a name="items" />
## Items

| name | key | type |
| ------------- |------------- |------------- |
| Number of AP | ruckusSystemStatsNumAP | SNMP_AGENT |
| Number of associated client devices | ruckusSystemStatsNumSta | SNMP_AGENT |
| Total received bytes of wireless interfaces | ruckusSystemStatsWLANTotalRxBytes | SNMP_AGENT |
| Total received multicast packets of wireless interfaces | ruckusSystemStatsWLANTotalRxMulticast | SNMP_AGENT |
| Total received packets of wireless interfaces | ruckusSystemStatsWLANTotalRxPkts | SNMP_AGENT |
| Total transmitted bytes of wireless interfaces | ruckusSystemStatsWLANTotalTxBytes | SNMP_AGENT |
| Total transmitted fail packets of wireless interfaces | ruckusSystemStatsWLANTotalTxFail | SNMP_AGENT |
| Total transmitted multicast packets of wireless interfaces | ruckusSystemStatsWLANTotalTxMulticast | SNMP_AGENT |
| Total transmitted packets of wireless interfaces | ruckusSystemStatsWLANTotalTxPkts | SNMP_AGENT |
| Total transmitted retry packets of wireless interfaces | ruckusSystemStatsWLANTotalTxRetry | SNMP_AGENT |

<a name="discoveries" />
## Discoveries

| name | key | type | delay |
| ------------- |------------- |------------- |------------- |
| Ruckus APs | APRZ-[{#SNMPVALUE}] | SNMP_AGENT | 1h |
| Ruckus SSIDs | SSIDRZ-[{#SNMPVALUE}] | SNMP_AGENT | 1h |

<a name="discovery_ruckus_aps" />
## Discovery Ruckus APs

### Items

| name | key | type |
| ------------- |------------- |------------- |
| AP {#AP_NAME}: Configuration Status | ruckusSCGAPConfigStatus[{#SNMPINDEX}] | SNMP_AGENT |
| AP {#AP_NAME}: Connection Status | ruckusSCGAPConnStatus[{#SNMPINDEX}] | SNMP_AGENT |
| AP {#AP_NAME}: Total number of terminal using this AP | ruckusSCGAPNumSta[{#SNMPINDEX}] | SNMP_AGENT |
| AP {#AP_NAME}: Received bytes | ruckusSCGAPRXBytes[{#SNMPINDEX}] | SNMP_AGENT |
| AP {#AP_NAME}: Transmitted bytes | ruckusSCGAPTXBytes[{#SNMPINDEX}] | SNMP_AGENT |

<a name="discovery_ruckus_ssids" />
## Discovery Ruckus SSIDs

### Items

| name | key | type |
| ------------- |------------- |------------- |
| SSID {#SSID_NAME}: Number of client devices | ruckusSCGWLANNumSta[{#SNMPINDEX}] | SNMP_AGENT |
| SSID {#SSID_NAME}: Received bytes | ruckusSCGWLANRxBytes[{#SNMPINDEX}] | SNMP_AGENT |
| SSID {#SSID_NAME}: Transmitted bytes | ruckusSCGWLANTxBytes[{#SNMPINDEX}] | SNMP_AGENT |
