# SNMP Hirschmann classic led
TemplateSNMP Hirschmann classic led made by automate@izi-it
Hash: xxxxxxxxxxxxxxx
## Summary
* [discoveries](#discoveries)
  * [Discovery Hirschmann classic ledoctgroup ](#discovery_hirschmann_classic_ledoctgroup
)  * [Discovery Hirschmann classic ledrsgroup ](#discovery_hirschmann_classic_ledrsgroup
)  * [Discovery Hirschmann classic ledrsrgroup ](#discovery_hirschmann_classic_ledrsrgroup
)
<a name="discoveries" />
## Discoveries

| name | key | type | delay |
| ------------- |------------- |------------- |------------- |
| Hirschmann classic ledoctgroup | hmLEDOctGroup-[{#SNMPVALUE}] | SNMP_AGENT | 1m |
| Hirschmann classic ledrsgroup | hmLEDRSGroup-[{#SNMPVALUE}] | SNMP_AGENT | 1m |
| Hirschmann classic ledrsrgroup | hmLEDRSRGroup-[{#SNMPVALUE}] | SNMP_AGENT | 1m |

<a name="discovery_hirschmann_classic_ledoctgroup" />
## Discovery Hirschmann classic ledoctgroup

### Items

| name | key | type |
| ------------- |------------- |------------- |
| LED {#LED}: State Fault | hmLEDOctFault[{#SNMPINDEX}] | SNMP_AGENT |
| LED {#LED}: Power Supply 1 State | hmLEDOctPowerSupply1[{#SNMPINDEX}] | SNMP_AGENT |
| LED {#LED}: Power Supply 2 State | hmLEDOctPowerSupply2[{#SNMPINDEX}] | SNMP_AGENT |
| LED {#LED}: Status Redundancy Manager | hmLEDOctRedundancyManager[{#SNMPINDEX}] | SNMP_AGENT |

<a name="discovery_hirschmann_classic_ledrsgroup" />
## Discovery Hirschmann classic ledrsgroup

### Items

| name | key | type |
| ------------- |------------- |------------- |
| LED {#LED}: Status Fault | hmLEDRSFault[{#SNMPINDEX}] | SNMP_AGENT |
| LED {#LED}: Power Supply State | hmLEDRSPowerSupply[{#SNMPINDEX}] | SNMP_AGENT |
| LED {#LED}: Status Redundancy Manager | hmLEDRSRedundancyManager[{#SNMPINDEX}] | SNMP_AGENT |
| LED {#LED}: Status Standby | hmLEDRStandby[{#SNMPINDEX}] | SNMP_AGENT |

<a name="discovery_hirschmann_classic_ledrsrgroup" />
## Discovery Hirschmann classic ledrsrgroup

### Items

| name | key | type |
| ------------- |------------- |------------- |
| LED {#LED}: State Fault | hmLEDRSRFault[{#SNMPINDEX}] | SNMP_AGENT |
| LED {#LED}: Power Supply State | hmLEDRSRPowerSupply[{#SNMPINDEX}] | SNMP_AGENT |
| LED {#LED}: State Redundancy Manager | hmLEDRSRRedundancyManager[{#SNMPINDEX}] | SNMP_AGENT |
| LED {#LED}: State Relay 1 | hmLEDRSRRelay1[{#SNMPINDEX}] | SNMP_AGENT |
| LED {#LED}: State Relay 2 | hmLEDRSRRelay2[{#SNMPINDEX}] | SNMP_AGENT |
| LED {#LED}: State Standby | hmLEDRSRStandby[{#SNMPINDEX}] | SNMP_AGENT |
