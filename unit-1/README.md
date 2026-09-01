# Unit 1: Cybersecurity Fundamentals & Security by Design

## Overview
This repository section covers core cybersecurity principles, threat actor behaviors, vulnerability dynamics across critical sectors, and the fundamental principles of **Security by Design**.

---

## 1. Understand Cyber Security

### Unit 1 - Q1: Describe the concepts of cyber security
Cyber security is the practice of protecting systems, networks, programs, and data from digital attacks, unauthorized access, damage, or theft. Its core conceptual framework rests on the **CIA Triad**:

* **Confidentiality:** Ensuring sensitive information is accessible only to authorized personnel (e.g., using AES encryption, strict RBAC, multi-factor authentication).
* **Integrity:** Safeguarding the accuracy and completeness of data and systems against unauthorized modification or tampering (e.g., using cryptographic hashes like SHA-256, digital signatures).
* **Availability:** Guaranteeing that systems, networks, and data remain accessible to authorized users whenever needed (e.g., implementing redundancy, regular backups, DDoS mitigation).

Beyond the CIA Triad, cyber security encompasses **defense-in-depth** (layering controls across physical, technical, and administrative domains), risk management, continuous monitoring, and incident response.

---

### Unit 1 - Q2: Explain the importance of cyber security
Cyber security is critical due to society's overwhelming reliance on digital infrastructure and interconnected networks:
* **Protection of Sensitive Data:** Safeguards personally identifiable information (PII), intellectual property, financial records, and national security data from exposure.
* **Business Continuity & Financial Stability:** Prevents operational disruption caused by ransomware or malware, saving organizations millions in downtime, remediation, and ransom demands.
* **Preservation of Trust & Reputation:** Maintains customer confidence; a data breach severely damages brand value and customer retention.
* **Protection of Critical National Infrastructure (CNI):** Ensures the safe operation of energy grids, healthcare systems, water treatment plants, and transportation networks.

---

### Unit 1 - Q3: Describe the consequences and implications of inadequate cyber security

| Impact Domain | Consequences & Implications |
| :--- | :--- |
| **Financial** | Direct loss of funds, regulatory fines (e.g., GDPR penalties up to €20m or 4% of global turnover), ransom payouts, forensic cleanup costs, legal compensation. |
| **Operational** | System outages, loss of operational control, permanent data destruction, supply chain disruptions, delayed service delivery. |
| **Reputational** | Loss of consumer and investor trust, negative media coverage, devaluation of stock price, breach of contractual obligations with partners. |
| **Legal & Regulatory** | Lawsuits from affected customers/employees, regulatory audits, potential prosecution for negligence under data protection laws. |
| **Human & Safety** | Risk to life in critical environments (e.g., ransomware shutting down hospital surgical systems or compromising industrial control systems). |

---

## 2. Understand Core Terminology and Key Aspects of Cyber Security

### Unit 1 - Q4: Define core terminology used in cyber security
* **Vulnerability:** A weakness or flaw in software, hardware, procedure, or system design that could be exploited by a threat actor.
* **Threat:** Any potential event, person, or vector with the intent or capability to exploit a vulnerability and cause harm.
* **Risk:** The likelihood or probability of a threat exploiting a vulnerability combined with the financial, operational, or physical impact of that event ($Risk = Threat \times Vulnerability \times Impact$).
* **Exploit:** A piece of software, sequence of commands, or technical trick designed to take advantage of a vulnerability to cause unintended behavior.
* **Attack Surface:** The total sum of all possible points (endpoints, networks, code, human entry points) where an unauthorized user can attempt to enter or extract data.
* **Asset:** Any data, device, system, software, or component that holds value to an individual or organization.
* **Incident:** An assessed event that actualizes a threat and compromises the confidentiality, integrity, or availability of an information asset.

---

### Unit 1 - Q5: Explain the terms good actors and bad actors
* **Good Actors:** Authorized individuals or organizations operating ethically, legally, and defensively to build, maintain, audit, and secure IT infrastructure (e.g., security analysts, ethical hackers, system administrators).
* **Bad Actors (Threat Actors):** Individuals, groups, or entities that deliberately bypass security controls without authorization to compromise systems, steal data, disrupt operations, or inflict harm for malicious, financial, or political gain.

---

### Unit 1 - Q6: Distinguish typical behaviours of good actors and bad actors

| Feature | Good Actors | Bad Actors |
| :--- | :--- | :--- |
| **Authorization** | Operates strictly within scope, laws, and contracts | Operates without consent; bypasses access controls |
| **Disclosure** | Practices Coordinated Vulnerability Disclosure (CVD) | Exfiltrates, sells, or publicly dumps sensitive data |
| **Maintenance** | Documents changes, runs audits, applies security patches | Deploys malware, ransomware, and persistence scripts |
| **Operational Goal**| Protects availability and strengthens defenses | Evades detection, clears logs, and disrupts operations |

---

### Unit 1 - Q7: Explain the motivations of good actors and bad actors

* **Good Actors:**
  * **System Resilience & Defense:** Protecting assets, infrastructure, and user data from unauthorized access.
  * **Compliance & Duty of Care:** Meeting legal, industry (e.g., PCI-DSS, ISO 27001), and contractual safety standards.
  * **Knowledge Sharing & Research:** Improving global security posture through open-source tool creation, threat intelligence sharing, and bug bounties.

* **Bad Actors:**
  * **Financial Gain:** Theft of funds, extortion via ransomware, sale of stolen data on dark web marketplaces.
  * **Ideology / Hacktivism:** Promoting political, social, or religious agendas through defacement, leaks, or service disruption.
  * **Espionage (State-Sponsored):** Gathering intelligence, stealing trade secrets/IP, or gaining strategic advantages over foreign nations.
  * **Thrill-Seeking / Ego:** Demonstrating technical prowess or gaining notoriety within hacker communities.
  * **Revenge (Malicious Insiders):** Disgruntled employees seeking to damage company assets or retaliate against management.

---

### Unit 1 - Q8: Identify key sectors that are most vulnerable to a cyber-attack
1. **Healthcare:** Stores vast amounts of high-value personal/medical data (PHI) on legacy systems; zero tolerance for downtime makes them vulnerable to ransomware.
2. **Finance & Banking:** High-value target for direct monetary theft, wire fraud, and payment processor manipulation.
3. **Critical National Infrastructure (Energy, Water, Transport):** Uses legacy Operational Technology (OT) and SCADA systems integrated with modern IP networks, often lacking modern security controls.
4. **Education (Schools & Universities):** Open networks, decentralized administration, large user bases, and high turnover rates create sprawling attack surfaces.
5. **Government & Public Sector:** High-value repositories of citizen data and target for foreign espionage, hacktivism, and supply chain attacks.
6. **Retail & E-Commerce:** High volume of credit card transactions (PCI data) and supply chain integration points.

---

### Unit 1 - Q9: Compare the motivations for a cyber-attack in key sectors

| Sector | Primary Motivations | Threat Actor Types |
| :--- | :--- | :--- |
| **Healthcare** | **Extortion (Ransomware):** High pressure to pay quickly due to immediate threat to human life.<br>**Data Theft:** Medical records command high black-market prices. | Cybercriminals, Organized Crime |
| **Finance** | **Direct Financial Gain:** Theft of funds, transaction interception.<br>**Corporate Espionage:** Market manipulation, proprietary trading code theft. | Cybercriminals, Insiders, Competitors |
| **Critical Infrastructure** | **Geopolitical Disruption:** System crippling during geopolitical conflict.<br>**Espionage:** Mapping operational technology for future sabotage. | Nation-State Actors (APTs) |
| **Government** | **Intelligence Gathering:** Stealing secret communications, defense data.<br>**Political Disruption:** Defacement, interfering with elections or public trust. | Nation-State Actors, Hacktivists |

---

### Unit 1 - Q10: Consider how an actor may carry out a cyber-attack
Threat actors typically execute attacks through a structured progression, such as the **Cyber Kill Chain**:

1. **Reconnaissance:** Gathering target intelligence via public records, open-source intelligence (OSINT), network scanning (Nmap), and social media profiling.
2. **Initial Access / Weaponization:** Crafting an exploit paired with a delivery mechanism (e.g., a phishing email containing a malicious PDF payload, exploiting an unpatched web application vulnerability).
3. **Execution & Delivery:** Convincing a user to run the file (phishing) or executing remote code on a vulnerable server (RCE).
4. **Persistence & Escalation:** Creating backdoor access (adding admin accounts, registry keys, scheduled tasks) and escalating privileges to gain domain control.
5. **Lateral Movement:** Pivoting across internal networks to locate critical assets and databases.
6. **Actions on Objectives:** Exfiltrating sensitive files, encrypting data with ransomware, or disrupting systems.

---

## 3. Understand Security by Design Principles

### Unit 1 - Q11: Describe the term security by design
**Security by Design** is an engineering approach in which cybersecurity controls, risk management, and defensive mechanisms are intentionally planned, architected, and built into software, hardware, and networks from the initial conceptual stage, rather than added reactively post-development or post-deployment.

---

### Unit 1 - Q12: Explore the principles of security by design
* **Least Privilege:** Users, applications, and processes are granted only the minimum access rights and permissions required to perform their specific function.
* **Defense-in-Depth:** Implementing multiple, overlapping layers of defense (e.g., firewall + network segmentation + MFA + endpoint protection) so that if one layer fails, others contain the threat.
* **Fail Securely:** When a system or application encounters an error or crashes, it should default to a state that denies access rather than leaving doors open.
* **Complete Mediation:** Every access request to every object must be verified and authorized every time, eliminating cached or assumed trust (aligned with **Zero Trust**).
* **Open Design:** Security mechanisms should rely on robust algorithms and architectures, not secrecy ("security through obscurity").
* **Keep Security Simple (KISS):** Avoid overly complex architectures; simpler designs reduce the attack surface and are easier to audit and maintain.
* **Minimize Attack Surface:** Disabling unused services, ports, APIs, and features to reduce entry points for attackers.

---

### Unit 1 - Q13: State the consequences of not considering cyber security during the design phase
* **Inherent System Vulnerabilities:** Structural design flaws (e.g., hardcoded credentials, cleartext communication) that are difficult or impossible to fix with simple patches later.
* **Exponentially Higher Costs:** Fixing architectural security flaws post-release requires extensive code rewrites, re-testing, downtime, and expensive emergency patches.
* **Increased Vulnerability Window:** Systems are exposed to zero-day exploits and attacks immediately upon deployment.
* **Compliance Failure:** Inability to meet regulatory standards (e.g., GDPR, NIS 2), leading to legal penalties and deployment blocks.
* **Patch Instability:** Applying security "band-aids" to legacy or poorly designed architectures frequently breaks non-security functionalities.

---

### Unit 1 - Q14: Evaluate the advantages and disadvantages of security by design

| **Advantages** | **Disadvantages** |
| :--- | :--- |
| **Proactive Risk Reduction:** Identifies and eliminates core architectural flaws before software goes into production. | **Higher Upfront Investment:** Increases initial planning, architectural scoping, and early-phase development costs. |
| **Long-Term Cost Savings:** Cheaper to build securely upfront than to retrofit, patch, or deal with data breach remediation later. | **Slower Initial Time-to-Market:** Rigorous security reviews, threat modeling, and testing delay early software releases. |
| **Enhanced Regulatory Compliance:** Built-in compliance mechanisms streamline audits for frameworks like GDPR, HIPAA, and ISO 27001. | **Increased Technical Complexity:** Requires developer security training, cross-team coordination, and specialized threat modeling tools. |
| **Resilience & Maintenance:** Systems are easier to patch, update, and maintain over their lifecycle. | **Usability Friction:** Strict default security controls (e.g., multi-step authentication) can degrade user experience if designed poorly. |
