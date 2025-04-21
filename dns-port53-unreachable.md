# Cybersecurity Incident Report: 

# Network Traffic Analysis

| Part 1: Provide a summary of the problem found in the DNS and ICMP  traffic log.  |  |
| :---- | ----- |
| The UDP protocol reveals that port 53 which is a port of DNS service is unreachable because no service was listening on the receiving DNS port. This is based on the results of the network analysis, which show that the ICMP echo reply returned the error message “udp port 53 unreachable”. The port noted in the error message is used for communication, that is, for sending and receiving queries. The most likely issue is that port 53 is either closed or being filtered by a firewall or network security service.  |  |
|  |  |

| Part 2: Explain your analysis of the data and provide at least one cause of the incident. |
| :---- |
| The IT team were made aware by customers of clients that kept complaining about not being able to access the website. They claimed that they kept seeing the error message "destination port unreachable" after waiting for the page to load.  The IT analyst tried to access the website and got the same error "destination port unreachable". To find the reason for the error, the analyst ran tests with the network protocol analyzer tool tcpdump while trying to load the website. The browser sent a query to the DNS server via the UDP protocol to retrieve the IP address for the website, www.yummyrecipesfome.com, domain name. The analyzer reveals that when the UDP packets were sent to the DNS server, ICMP packets containing the error message "udp port 53 unreachable" were received. This indicates that port 53 which is needed for translating the domain name into an IP address is not reachable. The most likely cause of the accident could be that the port is either closed or filtered by a firewall or network security device. This prevented DNS communication from taking place.  |

