# Detection, response & analysis
Disaster Recovery Planning and Strategies

## Key-terms
- Social engineering: The manipulation of individuals to divulge confidential information or perform actions that compromise security.
- Intrusion Detection System (IDS): A security tool that monitors network or system activities for malicious activities or policy violations and produces alerts.
- Intrusion Prevention System (IPS): A security tool that monitors network or system activities and can take actions to prevent detected incidents.
- Recovery Point Objective (RPO): The maximum acceptable amount of data loss measured in time before a disaster or outage.
- Recovery Time Objective (RTO): The maximum acceptable downtime for restoring services after a disaster or outage.
- Systems hardening: The process of securing a system by reducing its vulnerabilities and attack surface.
- Disaster recovery options: Strategies and plans for restoring systems and data following a disaster or outage.

## Opdracht
**Disaster Recovery Planning and Strategies**

**1. IDS and IPS:**
   - IDS and IPS are critical components of network security infrastructure.
   - IDS monitors network traffic for suspicious activity, while IPS can take automated actions to block or mitigate detected threats.

**2. Hack response strategies:**
   - Following an attack, organizations must respond swiftly to contain the damage and prevent further compromise.
   - Response strategies may include isolating affected systems, patching vulnerabilities, and investigating the root cause of the attack.

**3. Systems hardening:**
   - Systems hardening involves configuring systems to minimize security vulnerabilities and protect against potential threats.
   - This may include disabling unnecessary services, implementing access controls, and regularly updating software and firmware.

**4. Disaster recovery options:**
   - Disaster recovery options range from simple backups to redundant infrastructure setups.
   - Strategies include cold backups, hot backups, failover systems, and redundant sites, each with different costs and levels of resilience.

**Exercise:**
1. **RPO of the database:**
   - The database is automatically recovered using the most recent backup on a different physical machine in 15 minutes.
   - Since the recovery happens using the most recent available backup, the RPO is equal to the time interval between backups. In this case, it's one day, assuming daily backups. So, the RPO of the database is 1 day.

2. **RTO of the website:**
   - The automatic failover to a backup web server takes about 8 minutes to complete.
   - RTO is the maximum acceptable downtime for restoring services. In this case, it's 8 minutes.

## Gebruikte bronnen
- Understanding Recovery Point Objective (RPO) and Recovery Time Objective (RTO): [Link](https://www.veeam.com/blog/rto-rpo-executive-guide-disaster-recovery.html)
- Overview of IDS and IPS: [Link](https://www.cloudflare.com/learning/security/glossary/intrusion-detection-system-ids/)
- Guide to Systems Hardening: [Link](https://www.sans.org/security-resources/idfaq/hardening.php)
- Different Disaster Recovery Options: [Link](https://www.zetta.com/blog/4-disaster-recovery-options-which-right-your-business)

## Ervaren problemen
No significant problems were encountered in understanding and explaining the concepts related to disaster recovery planning and strategies.

## Resultaat
The success of the exercise can be confirmed by calculating the RPO and RTO values based on the provided scenarios. Additionally, understanding the key concepts and strategies involved in disaster recovery planning indicates the successful completion of the assignment.