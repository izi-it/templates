# SNMP Athonet epc lte
Template SNMP Athonet epc lte made by automate@izi-it
Hash: xxxxxxxxxxxxxxx

Check aggregate statistics.
## Summary
* [items](#items)

<a name="items" />
## Items

| name | key | type |
| ------------- |------------- |------------- |
| Number of succesfull PDN context activation | lteActivatedPDNContext | SNMP_AGENT |
| Number of active sessions from users | lteActiveConnections | SNMP_AGENT |
| Incoming traffic going through the interface | lteLoadPktInGi | SNMP_AGENT |
| Outgoing traffic going through the interface | lteLoadPktOutGi | SNMP_AGENT |
| Number of PDN Context reject - Insufficent Resources | ltePDNRejInsufRes | SNMP_AGENT |
| Number of PDN Context reject - Missing or unknown APN | ltePDNRejNoApn | SNMP_AGENT |
| Number of PDN Context reject - Request service option not subscribed | ltePDNRejNoSubscribed | SNMP_AGENT |
| Number of succesfull attach request | lteSuccesfullAttach | SNMP_AGENT |
| Number total of attach request | lteTotalAttachReq | SNMP_AGENT |
| Number total of PDN | lteTotalPDNActReq | SNMP_AGENT |
| Number of UE context request release | lteUERelReq | SNMP_AGENT |
| Number of UE context request release - Radio Connection with UE lost | lteUERelReqRadioLost | SNMP_AGENT |
| Number of connected users | lteUsersConnected | SNMP_AGENT |
| Number of idle users | lteUsersIdle | SNMP_AGENT |
