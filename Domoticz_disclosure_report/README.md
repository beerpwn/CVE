# Domoticz vulnerabilities disclosure

## Author: bytevsbyte

* CVE-2019-10664 (Unauthenticated SQL Injection)
* CVE-2019-10678 (Command Injection)

[_THIS PDF_](./Report_Domoticz.pdf) is the report that I've shared with the maintainers. It shows all the POC to reproduce the issues, with a short description for each of the security flaw.

The chain of the two vulnerabilities lead to a Remote Command Execution from not authenticated. I published an exploit on exploit-db: [_Domoticz 4.10577 - Unauthenticated Remote Command Execution_](https://www.exploit-db.com/exploits/46773)

__bytevsbyte (twitter @bytevsbyt3)__
