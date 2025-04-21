**Incident report analysis**

**Instructions**

As you continue through this course, you may use this template to record your findings after completing an activity or to take notes on what you've learned about a specific tool or concept. You can also use this chart as a way to practice applying the NIST framework to different situations you encounter.

| Summary | The company experienced a Distributed Denial of Service (DDoS) attack that disrupted internal network services for approximately two hours. The attack exploited an unconfigured firewall, allowing a flood of ICMP packets to overwhelm the network. As a result, internal services were inaccessible. The incident was mitigated by blocking ICMP traffic, restoring critical services, and conducting a security analysis. The following plan is based on the NIST Cybersecurity Framework to strengthen the company’s network security posture. |  |  |
| :---- | :---- | ----- | ----- |
| Identify | The analyst conducted an audit. They checked the systems, devices and access policies involved in the attack to identify the gaps in security. From the audit conducted, it was concluded that a malicious attacker overwhelmed the network of the company through a Distributed Denial of Service (DDoS) Attack. The audit also exposed weak firewall rules and lack of proper traffic filtering. |  |  |
| Protect | To protect the network, the network security implemented: 1\. A new firewall rule to limit the rate of incoming ICMP packets. 2\. Source IP address verification on the firewall to check for spoofed IP addresses on incoming ICMP packets. 3\. Network monitoring software to detect abnormal traffic patterns. 4\. An IDS/IPS system to filter out some ICMP traffic based on suspicious characteristics. 5\. Employee training on security protocols and awareness. 6\. Ongoing patch updates and port filtering to reduce exposure to known vulnerabilities. |  |  |
| Detect | To detect another attack of the same type or any kind in the future, the team should ensure firewall maintenance to keep it up to date and an IDS/IPS to monitor and prevent the attack in the future. Utilize network log analysis tools, such as a SIEM (Security Information and Event Management) system, to analyze logs and detect anomalies. |  |  |
| Respond | Subnetting helps isolate parts of the network, limiting the impact of an attack and preventing it from affecting critical services. By splitting the network into smaller subnets, the attack can be contained, and only affected subnets would require intervention, while others remain operational. |  |  |
| Recover | After the DDoS attack, critical services were restored, and patches and configuration fixes were applied to the affected systems. The incident response and recovery processes were reviewed to ensure readiness for any future attacks. The team would also review logs to learn from the attack and improve future responses. |  |  |

---

| Reflections/Notes: |
| :---- |

