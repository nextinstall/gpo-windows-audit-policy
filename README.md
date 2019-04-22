# gpo-windows-audit-policy
A GPO that can be imported which will enable robust auditing for Windows Servers based off Microsoft best practices and Center for Internet Security recommendations.

## DC Audit Policy

ENables PowerShell Script Block auditing!

also Contains NTLM auditing: 

```
MACHINE\System\CurrentControlSet\Control\Lsa\MSV1_0\AuditReceivingNTLMTraffic=4,2
MACHINE\System\CurrentControlSet\Services\Netlogon\Parameters\AuditNTLMInDomain=4,7
```

|Subcategory	|   Inclusion Setting   |
|------------|------------|
Audit Credential Validation	|   Success and Failure
Audit Kerberos Authentication Service   |	Success and Failure
Audit Kerberos Service Ticket Operations    |	Success and Failure
Audit Other Account Logon Events    |	Success and Failure
Audit Application Group Management	|   Success and Failure
Audit Computer Account Management	|   Success and Failure
Audit Distribution Group Management	|   Success and Failure
Audit Other Account Management Events	|   Success and Failure
Audit Security Group Management	    |   Success and Failure
Audit User Account Management	|   Success and Failure
Audit DPAPI Activity	|   Success and Failure
Audit Process Creation	|   Success and Failure
Audit Directory Service Access  |	Success and Failure
Audit Directory Service Changes	|   Success and Failure
Audit Account Lockout	|   Success
Audit Logoff    |	Success
Audit Logon	|   Success and Failure
Audit Other Logon/Logoff Events	    | Success and Failure
Audit Special Logon |	Success and Failure
Audit Audit Policy Change	|   Success and Failure
Audit Authentication Policy Change	|   Success and Failure
Audit MPSSVC Rule-Level Policy Change   |	Success
Audit IPsec Driver  |	Success and Failure
Audit Other System Events	|   Success and Failure
Audit Security State Change	    |   Success and Failure
Audit Security System Extension	|   Success and Failure
Audit System Integrity  |	Success and Failure


## Member Server Audit Policy

