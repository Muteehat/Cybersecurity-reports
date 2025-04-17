# Security incident report

| Section 1: Identify the network protocol involved in the incident |  |
| :---- | ----- |
| The DNS and HTTP protocol were involved in the incident. Domain Name System (DNS): the browser requests the IP address of yummyrecipesforme.com and greatrecipesforme.com from DNS. HTTP (Hypetext Transfer Protocol): used to request web pages using the IP address sent by the DNS server to download the malicious executable file. |  |
|  |  |

| Section 2: Document the incident |
| :---- |
| The problem was reported by multiple customers of yummyrecipesforme.com. Their complaint was that the company's website had prompted them to download an executable file to access free recipes which changed the address of the website when run. This caused their personal computers to run slowly.  After analyzing the problem, the analyst found that a former employer used brute force to gain access to the web host using default passwords for the administrative account. After gaining access, the attacker altered the website's source code by adding a JavaScript function that asked the users to download an executable file with malware in it. Once run, the file redirected the users to a different website, greatrecipesforme.com, resulting in performance issues and system compromise. The analyst used the tcpdump analyser tool to analyse the DNS and HTTP traffic, confirming the problem reported by the users. The process include:  1\. Browser requesting for IP address of the yummyrecipesforme.com URL from the DNS server and the DNS replies with the correct IP address. 2\. HTTP requests the download of the file. 3\. The browser requests for the domain of the fake websites, greatrecipeforme.com, after the file is run. The browser is then redirected to the website. The cause of the problem is mainly weak security, weak password policy and lack of firewall . To prevent such an incident from happening again, strong password policies should be implemented, install a firewall, stop the use of default passwords, and use IDS/IPS to monitor login behavior. |

| Section 3: Recommend one remediation for brute force attacks |
| :---- |
| Installation of a firewall  |

