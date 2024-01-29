# SNMP Audiocodes module
Template SNMP Audiocodes module by automate@izi-it
Hash: xxxxxxxxxxxxxxx

Template to check Audiocodes equipments using SNMP protocol
## Summary
* [discoveries](#discoveries)
  * [Discovery Audiocodes module ](#discovery_audiocodes_module
)
<a name="discoveries" />
## Discoveries

| name | key | type | delay |
| ------------- |------------- |------------- |------------- |
| Audiocodes module | acSysModuleIndex-[{#SNMPVALUE}] | SNMP_AGENT | 5m |

<a name="discovery_audiocodes_module" />
## Discovery Audiocodes module

### Items

| name | key | type |
| ------------- |------------- |------------- |
| Module {#MODULE_INDEX}: Status | acSysModuleFRUstatus[{#SNMPINDEX}] | SNMP_AGENT |
| Module {#MODULE_INDEX}: Existence | acSysModulePresence[{#SNMPINDEX}] | SNMP_AGENT |
