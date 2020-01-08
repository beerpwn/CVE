# ioBroker vulnerabilities disclosure

## Author: bytevsbyte

* CVE-2019-10765 (Directory Traversal on iobroker.admin)
* CVE-2019-10767 (Directory Traversal on iobroker.js-controller -> lead to RCE)
* CVE-2019-10771 (XSS reflected on iobroker.web)

The report sent to the maintainers is [HERE](./Report_iobroker.pdf).\
It shows all the POC to reproduce the issues, with a short description for each security flaw.
Note that if the authentication is enabled (not the default) you have to be logged in to exploit the two directory traversal.

bytevsbyte (twitter @bytevsbyt3)
