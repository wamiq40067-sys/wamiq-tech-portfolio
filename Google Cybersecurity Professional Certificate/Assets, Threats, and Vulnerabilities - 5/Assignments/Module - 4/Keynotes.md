# Key Notes: Social Engineering, Malware, Web-Based Exploits, and Threat Modeling

# Social Engineering

* Social engineering is a manipulation technique used to exploit human behavior to gain unauthorized access, information, or valuables.
* Attackers often rely on trust, fear, curiosity, urgency, or rewards to deceive victims.
* These attacks usually bypass technical defenses by targeting human weaknesses instead of software vulnerabilities.

## Common Social Engineering Attacks

* **Phishing:** Fraudulent emails or messages used to steal information or spread malware.
* **Smishing:** Phishing attacks performed through text messages or messaging apps.
* **Vishing:** Voice-based phishing attacks conducted over phone calls or voice messages.
* **Spear phishing:** Highly targeted phishing attacks aimed at specific individuals or organizations.
* **Whaling:** Spear phishing attacks focused on executives or senior officials.
* **Baiting:** Offering something tempting to trick users into compromising security.
* **Quid pro quo:** Promising rewards or benefits in exchange for sensitive information.
* **Tailgating:** Unauthorized individuals following authorized personnel into restricted areas.
* **Watering hole attack:** Compromising websites frequently visited by targeted users.
* **Angler phishing:** Attackers impersonating customer service representatives on social media.

## Prevention Techniques

* Verify suspicious emails, calls, and messages.
* Avoid clicking unknown links or attachments.
* Use multi-factor authentication (MFA).
* Limit oversharing on social media.
* Provide security awareness training to employees and users.

---

# Malware

* Malware is malicious software created to damage systems, steal information, disrupt operations, or gain unauthorized access.
* Malware infections commonly spread through phishing emails, malicious downloads, infected websites, and vulnerable applications.

## Common Types of Malware

### Virus

* Requires user interaction to activate.
* Infects files or software and spreads between systems.

### Worm

* Self-replicates and spreads across networks automatically.
* Often targets shared systems and connected devices.

### Trojan Horse

* Disguised as legitimate software or files.
* Tricks users into installing malicious programs.

### Adware

* Displays advertisements within software.
* Malicious adware may track activity or install unwanted applications.

### Spyware

* Secretly collects user data without consent.
* Often bundled with free software.

### Scareware

* Uses fake warnings or alerts to frighten users into installing malware.

### Fileless Malware

* Operates in system memory without installing files on the hard drive.
* Uses legitimate system tools to avoid detection.

### Rootkit

* Provides hidden administrative access to attackers.
* Often used to maintain long-term control over systems.

### Ransomware

* Encrypts files or systems and demands payment for recovery.

### Cryptojacking

* Secretly uses system resources to mine cryptocurrency.

### Botnet

* A group of infected devices controlled remotely by a threat actor.

## Malware Prevention

* Keep operating systems and applications updated.
* Use antivirus and endpoint protection tools.
* Avoid downloading files from untrusted sources.
* Monitor systems for suspicious activity.
* Regularly back up important data.

---

# Web-Based Exploits

* Web-based exploits target vulnerabilities in websites and web applications.
* Attackers exploit coding flaws to steal data, gain access, or execute malicious actions.

## Common Web-Based Attacks

### SQL Injection

* Malicious SQL code is inserted into vulnerable input fields.
* Can allow attackers to access, modify, or delete database information.

### Cross-Site Scripting (XSS)

* Attackers inject malicious scripts into websites.
* Scripts execute in users’ browsers and may steal session data or credentials.

#### Types of XSS

* **Stored XSS:** Malicious scripts are permanently stored on the server.
* **Reflected XSS:** Scripts are reflected from the server through user requests.
* **DOM-based XSS:** Scripts manipulate the browser’s Document Object Model (DOM).

## Prevention Methods

* Use input validation and input sanitization.
* Implement prepared statements for database queries.
* Escape user-generated content.
* Apply secure coding practices.
* Conduct regular vulnerability assessments and patch management.

---

# Threat Modeling

* Threat modeling is the process of identifying assets, vulnerabilities, threats, and risks within a system or application.
* It helps organizations proactively improve security before attacks occur.
* Threat modeling is commonly integrated into the Software Development Lifecycle (SDLC).

## Threat Modeling Process

1. Define the system scope
2. Identify assets and threats
3. Analyze the operating environment
4. Assess vulnerabilities and risks
5. Apply mitigation strategies
6. Evaluate and improve security controls

## Common Threat Modeling Frameworks

### STRIDE

Focuses on six threat categories:

* Spoofing
* Tampering
* Repudiation
* Information disclosure
* Denial of service
* Elevation of privilege

### PASTA

* Risk-focused framework for attack simulation and threat analysis.
* Uses evidence-based assessments.

### Trike

* Security-centered framework focusing on permissions, access control, and risk management.

### VAST

* Automated and scalable threat-modeling framework integrated with agile environments.

## Importance of Threat Modeling

* Helps identify security weaknesses early.
* Reduces application and business risks.
* Improves secure software development practices.
* Supports proactive cybersecurity defense strategies.

---
