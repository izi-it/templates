# SNMP Checkpoint disk
Template to check Checkpoint disk equipments using SNMP protocol by izi-it
## Summary
* [discoveries](#discoveries)
  * [Discovery Checkpoint disk ](#discovery_checkpoint_disk
)
<a name="discoveries" />
## Discoveries

| name | key | type | delay |
| ------------- |------------- |------------- |------------- |
| Checkpoint disk | multiDiskName-[{#SNMPVALUE}] | SNMP_AGENT | 1h |

<a name="discovery_checkpoint_disk" />
## Discovery Checkpoint disk

### Items

| name | key | type |
| ------------- |------------- |------------- |
| Disk {#DISK_NAME}: Total space | multiDiskSize[{#SNMPINDEX}] | SNMP_AGENT |
| Disk {#DISK_NAME}:Used space (%) | multiDiskUsedPercent[{#SNMPINDEX}] | CALCULATED |
| Disk {#DISK_NAME}: Used space | multiDiskUsed[{#SNMPINDEX}] | SNMP_AGENT |

### Triggers

| name | expression | priority |
| ------------- |------------- |------------- |
| {#DISK_NAME}: Disk space is critically low | min(/SNMP Checkpoint disk/multiDiskUsedPercent[{#SNMPINDEX}],5m)>{$_CRITDISK} | HIGH |
| {#DISK_NAME}: Disk space is warning low | min(/SNMP Checkpoint disk/multiDiskUsedPercent[{#SNMPINDEX}],5m)>{$_WARNDISK}<br>and min(/SNMP Checkpoint disk/multiDiskUsedPercent[{#SNMPINDEX}],5m)<{$_CRITDISK} | WARNING |
