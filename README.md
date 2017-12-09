# Invoke-WCMDump
PowerShell Script to Dump Windows Credentials from the Credential Manager

Enumerates Windows credentials in the Credential Manager and then extracts available information about each one. Passwords are retrieved for "Generic" type credentials, but can not be retrived by the same method for "Domain" type credentials.

## Example
```
PS>Import-Module .\Invoke-WCMDump.ps1
PS>Invoke-WCMDump
    Username         : testusername
    Password         : P@ssw0rd!
    Target           : TestApplication
    Description      :
    LastWriteTime    : 12/9/2017 4:46:50 PM
    LastWriteTimeUtc : 12/9/2017 9:46:50 PM
    Type             : Generic
    PersistenceType  : Enterprise
```
