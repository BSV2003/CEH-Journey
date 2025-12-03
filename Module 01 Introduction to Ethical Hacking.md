# Module 01 – Introduction to Ethical Hacking

## 🎯 Learning Objectives

At the end of this module, you should be able to:
- Describe the elements of information security  
- Explain information security attacks and information warfare  
- Understand hacking concepts and hacker classifications  
- Explain ethical hacking concepts and AI-driven ethical hacking  
- Describe hacking methodologies and frameworks  
- Understand key information security controls:
  - Information assurance  
  - Defense-in-depth  
  - Risk management  
  - Cyber threat intelligence  
  - Threat modeling  
  - Incident management  
  - AI/ML  
- Understand various information security acts and laws  

---

## 🧨 Why Study Ethical Hacking?

Attackers break into systems for many reasons—financial gain, espionage, disruption, thrill, revenge, etc.  
To defend systems effectively, security professionals must understand:
- How attackers think  
- How they exploit systems  
- Why they attack  

As Sun Tzu said in *The Art of War*:  
**“Know your enemy.”**

---

# 🔐 Information Security Concepts

Information security refers to the protection of information and information systems that **store, process, and transmit data**, preventing:
- Unauthorized access  
- Disclosure  
- Alteration  
- Destruction  

Information is a critical asset. If compromised, an organization may face:
- Financial loss  
- Reputation damage  
- Customer loss  
- Legal consequences  

This section introduces the **5 elements of information security**.

---

## 🛡️ Elements of Information Security (CIAAN)

Information security is based on five foundational principles:

---

### 1️⃣ Confidentiality  
Ensures information is accessible **only to authorized individuals**.

**Controls include:**  
- Data classification  
- Data encryption  
- Secure disposal of devices  

Improper handling or hacking attempts may lead to confidentiality breaches.

---

### 2️⃣ Integrity  
Ensures data is **accurate, trustworthy, and unaltered**.

Integrity protects against:
- Unauthorized changes  
- Data corruption  
- Manipulation  

**Controls include:**  
- Checksums (to detect changes)  
- Access control (restrict who can update/delete data)

---

### 3️⃣ Availability  
Ensures systems are **accessible when needed** by authorized users.

**Measures include:**  
- Disk arrays (for Redundant systems and clustered machines)
- Antivirus protection (to combat malware)
- DDoS prevention systems  

---

### 4️⃣ Authenticity  
Ensures data, users, and communications are **genuine**.

**Controls include:**  
- Biometrics  
- Smart cards  
- Digital certificates  

Authenticity verifies that:
- A user is genuine  
- A transaction is legitimate  
- Data has not been tampered with  

---

### 5️⃣ Non-Repudiation  
Ensures that:
- The sender **cannot deny** sending a message  
- The receiver **cannot deny** receiving it  

**Digital signatures** are commonly used to provide non-repudiation.

---

# 🧨 Information Security Attacks: Motives, Goals & Objectives

An **attack** is any action performed with the intent to breach an IT system’s security by **exploiting its vulnerabilities**.

An attack may involve attempts to:
- Obtain information  
- Edit or manipulate information  
- Remove or destroy data  
- Implant malicious code  
- Reveal sensitive information  
- Cause unexpected behavior in software/hardware  

Attacks may also involve:
- Malicious software  
- Malicious commands  
- Scripts or payloads crafted to exploit weaknesses  

### ⚡ Attack Formula  
**Attacks = Motive (Goal) + Method (TTP) + Vulnerability**

This means every attack consists of:
- **A Goal:** *Why* the attacker wants to attack  
- **A Method / TTPs:** *How* the attacker executes the attack  
- **A Vulnerability:** *What* weakness is being exploited  

---

## 🎯 Motives (Goals) of Attackers

A motive arises when an attacker believes a system contains **something valuable** or vulnerable.  
Motives depend on:
- Attacker’s mindset  
- Purpose for the attack  
- Resources and capabilities  

Common motives include:

- Disrupt business continuity  
- Steal information (information theft)  
- Manipulate or alter data  
- Create fear or chaos by targeting critical infrastructures  
- Bring financial loss to the target  
- Propagate political or religious ideologies  
- Achieve military or strategic objectives  
- Damage the organization’s reputation  
- Take revenge  
- Demand ransom (extortion)  

---

## 🛠️ Tactics, Techniques, and Procedures (TTPs)

**TTPs** refer to the recognizable patterns, behaviors, and methods associated with specific threat actors or groups of attackers.

They help organizations:
- Analyze threats  
- Profile threat actors  
- Strengthen security infrastructure  
- Understand how attacks evolve  

TTPs consist of three components:

---

### 1️⃣ **Tactics**
- The **high-level strategy** or objective of the attacker  
- Describes *what* the attacker wants to achieve from start to finish  
- Example: persistence, privilege escalation, lateral movement  

Understanding tactics helps:
- Predict adversary behavior  
- Detect attacks in early stages  

---

### 2️⃣ **Techniques**
- The **general technical methods** used to accomplish a tactic  
- Represents *how* attackers achieve intermediate goals  
- Example: spear-phishing, credential dumping, exploiting services  

Understanding techniques helps:
- Identify potential vulnerabilities  
- Implement preventive controls  

---

### 3️⃣ **Procedures**
- The **detailed, step-by-step actions** attackers follow to execute a technique  
- Often specific to individual threat groups  
- Example: exact command sequences, tool configurations, exploit scripts  

Analyzing procedures helps:
- Reveal attacker intent  
- Understand what the attacker is searching for in a target environment  
- Improve incident response readiness  

---

## 💡 Why TTPs Matter
Studying TTPs allows defenders to:
- Anticipate attacker behavior  
- Implement proactive defenses  
- Improve detection mechanisms  
- Enhance threat intelligence  
- Build stronger security strategies based on real-world adversary patterns

---

# 🕳️ Vulnerabilities

A **vulnerability** is a weakness in the design, implementation, configuration, or use of a system that can be exploited to compromise its security.

A vulnerability may allow attackers to:
- Bypass authentication  
- Gain unauthorized access  
- Leak or manipulate data  
- Execute malicious commands  
- Cause abnormal system behavior  

There are two primary causes of vulnerabilities:
- **Hardware or software misconfiguration**
- **Poor programming practices**

Attackers exploit vulnerabilities to perform a wide range of cyber-attacks.

---

## 🧭 Common Reasons for the Existence of Vulnerabilities

### 1️⃣ Hardware or Software Misconfiguration
Insecure configuration creates security loopholes.
Examples:
- Unencrypted communication protocols  
- Incorrect access control settings  
- Misconfigured network services  

Misconfigurations can expose:
- Systems  
- Applications  
- Sensitive data  

---

### 2️⃣ Insecure or Poor Network/Application Design
Flawed architectural decisions can lead to data loss or system compromise.

Examples:
- Improperly configured firewalls  
- Weak IDS/IPS implementations  
- Poorly designed VPN configurations  

If security components are not deployed correctly, the entire network becomes vulnerable.

---

### 3️⃣ Inherent Technology Weaknesses
Some technologies naturally come with limitations or flaws.

Examples:
- Web browsers vulnerable to MITM attacks  
- Older software lacking modern security protections  
- Outdated OS versions prone to exploits (e.g., DoS attacks)

Failure to update or patch these technologies increases risk.

---

### 4️⃣ End-User Carelessness
Humans remain the weakest link in security.

Examples of careless behavior:
- Sharing login credentials  
- Falling for phishing/social engineering  
- Using weak passwords  
- Connecting to insecure networks  

Such actions can lead to:
- Data leakage  
- System compromise  
- Unintentional security breaches  

---

### 5️⃣ Intentional End-User Acts
Malicious actions performed intentionally by trusted users.

Example:
- Ex-employees accessing shared drives and leaking confidential data  

Consequences:
- Severe data loss  
- Financial damage  
- Legal risks  

---

# 🧪 Examples of Vulnerabilities

## 🖥️ Technological Vulnerabilities

| Vulnerability Type | Description |
|--------------------|-------------|
| **TCP/IP Protocol Vulnerabilities** | Protocols like HTTP, FTP, ICMP, SNMP, SMTP are inherently insecure. |
| **Operating System Vulnerabilities** | OS may be insecure or lacking the latest patches/updates. |
| **Network Device Vulnerabilities** | Routers, firewalls, switches may lack: password protection, authentication, secure routing, or have firewall weaknesses. |

---

## 🔧 Configuration Vulnerabilities

| Vulnerability Type | Description |
|--------------------|-------------|
| **User Account Vulnerabilities** | Insecure transmission or handling of credentials (usernames/passwords). |
| **System Account Vulnerabilities** | Weak passwords for system-level accounts. |
| **Internet Service Misconfiguration** | Incorrect configuration of services (IIS, Apache, FTP, Terminal services, JavaScript-enabled services). |
| **Default Passwords & Settings** | Using default device settings or factory credentials. |
| **Network Device Misconfiguration** | Incorrect configurations on routers, switches, firewalls, etc. |

---

# ⚔️ Classification of Attacks

According to the **Information Assurance Technical Framework (IATF)**, attacks are classified into **five major categories**:
1. Passive Attacks  
2. Active Attacks  
3. Close-in Attacks  
4. Insider Attacks  
5. Distribution Attacks  

---

## 1️⃣ Passive Attacks

A **passive attack** involves intercepting, capturing, or monitoring data flowing across a network **without altering it**.

Key characteristics:
- The attacker **does not modify** data or interact with the target system.
- Extremely **difficult to detect**, because there is no noticeable change in system behavior.
- Primarily used for **reconnaissance**, intelligence gathering, and preparing for active attacks.
- Attackers commonly use **packet sniffers** and network monitoring tools.

Passive attacks allow an attacker to capture:
- Unencrypted data in transit  
- Clear-text usernames and passwords  
- Sensitive information  
- Network details used for planning future attacks  

### 🔍 Examples of Passive Attacks
- **Footprinting**  
- **Sniffing and eavesdropping**  
- **Network traffic analysis**  
- **Decryption of weak or poorly encrypted traffic**  

---

## 2️⃣ Active Attacks

An **active attack** involves tampering with data, disrupting communication, or actively interacting with a system to compromise its security.

Key characteristics:
- The attacker **modifies**, **injects**, or **blocks** data.
- The attacker directly interacts with the network, making the attack **detectable**.
- These attacks aim to **exploit information in transit** or penetrate internal networks.
- Attackers may gain remote access, infect systems, or completely compromise the organization’s internal environment.

Active attacks can:
- Disrupt services  
- Alter or delete data  
- Inject malicious payloads  
- Bypass security controls  
- Escalate privileges  
- Steal sensitive information  

### 🔥 Examples of Active Attacks
- Denial-of-Service (DoS) attacks  
- Bypassing protection mechanisms  
- Malware attacks (viruses, worms, ransomware)  
- Modification of information  
- Spoofing attacks  
- Replay attacks  
- Password-based attacks  
- Session hijacking  
- Man-in-the-Middle (MITM) attack  
- DNS and ARP poisoning  
- Compromised-key attacks  
- Firewall and IDS attacks  
- Profiling and enumeration  
- Arbitrary code execution  
- Privilege escalation  
- Backdoor access  
- Cryptographic attacks  
- SQL injection  
- Cross-Site Scripting (XSS)  
- Directory traversal attacks  
- Exploitation of OS and application vulnerabilities  

---

## 3️⃣ Close-In Attacks

A **close-in attack** occurs when the attacker is in physical proximity to the target system or network.  
These attacks involve direct physical access or being near enough to observe or intercept sensitive information.

Key characteristics:
- Attacker must be **physically close** to the target  
- Goal is to **gather**, **modify**, or **disrupt** information or access  
- Proximity may be gained through:
  - Surreptitious entry (unauthorized physical access)
  - Open access (public areas, office spaces, shared environments)

Typical example:
- **Shoulder surfing** to capture user credentials

### 🕵️ Examples of Close-In Attacks
- Social engineering techniques:
  - Eavesdropping  
  - Shoulder surfing  
  - Dumpster diving  
  - Physical observation of sensitive activities  

---

## 4️⃣ Insider Attacks

An **insider attack** is carried out by trusted individuals who already have legitimate access to the organization’s systems, data, or physical environment.

Key characteristics:
- Performed by **employees, contractors, partners, or former staff**
- Attackers use **privileged access** to violate rules or cause intentional harm
- Insiders can bypass security measures more easily than external attackers
- These attacks can compromise:
  - Confidentiality  
  - Integrity  
  - Availability  

Insider attacks may severely impact:
- Business operations  
- Organizational reputation  
- Financial stability  

They are particularly **difficult to detect**, since insiders typically operate within authorized boundaries.

### 🕵️ Examples of Insider Attacks
- Eavesdropping and wiretapping  
- Theft of physical devices  
- Social engineering  
- Data theft and data destruction (spoliation)  
- Pod slurping (unauthorized copying of data to portable devices)  
- Planting keyloggers, backdoors, or malware  

---

## 5️⃣ Distribution Attacks

A **distribution attack** occurs when attackers tamper with hardware or software **before it reaches the end user**.  
This manipulation typically happens:
- At the source (manufacturer/vendor)
- During shipment or distribution  
- During supply chain handling  

The goal is to embed malicious components—such as **backdoors**, altered firmware, or compromised software—that give attackers unauthorized access once the product is deployed.

Distribution attacks are dangerous because:
- They compromise the integrity of systems **before installation**
- They often go undetected for long periods
- They affect large numbers of devices through the supply chain

### 🧪 Examples of Distribution Attacks
- Modification of hardware or software during **manufacturing**
- Modification of hardware or software during **distribution**  
- Pre-installed backdoors by malicious vendors  
- Tampered firmware shipped to organizations  

---

# ⚔️ Information Warfare (InfoWar)

**Information Warfare (InfoWar)** refers to the use of information and communication technologies (ICT) to gain a competitive advantage over an opponent.  
It involves using information as both a **weapon** and a **target**.

Common information warfare "weapons" include:
- Viruses, worms, Trojan horses  
- Logic bombs, trapdoors  
- Electronic jamming tools  
- Penetration tools and exploit frameworks  
- Nanomachines / micro attacks (theoretical/advanced)  

---

## 🧭 Categories of Information Warfare (Libicki’s Model)

### 1️⃣ Command and Control Warfare (C2 Warfare)
- Refers to the **degree of control** an attacker has over a compromised system or network.
- Involves disrupting or taking over the decision-making systems of the opponent.

---

### 2️⃣ Intelligence-Based Warfare
- Uses **sensor-based technologies** to corrupt or manipulate systems.
- Centers around protecting or denying access to knowledge needed to dominate the battlespace.
- Focuses on:
  - System corruption  
  - Knowledge disruption  
  - Information dominance  

---

### 3️⃣ Electronic Warfare
- Uses **radio-electronic** and **cryptographic** techniques to degrade or disrupt communication.
- Radio-based: Attacks the physical medium of communication (signals, frequencies)
- Crypto-based: Uses digital methods to disrupt or manipulate transmitted data.

---

### 4️⃣ Psychological Warfare
- Uses propaganda, misinformation, and fear tactics to demoralize or manipulate the opponent.
- Examples:
  - Threat messages  
  - Fake news  
  - Fear-inducing broadcasts  

---

### 5️⃣ Hacker Warfare
- Uses traditional hacking tools and malware to compromise digital infrastructure.
- Purposes include:
  - System shutdown  
  - Data theft or manipulation  
  - Monitoring  
  - False messaging  
  - Service theft  

Common tools:
- Viruses  
- Logic bombs  
- Trojan horses  
- Sniffers  

---

### 6️⃣ Economic Warfare
- Targets **financial systems** or **information flows** to damage a business or nation’s economy.
- Also includes blocking or disrupting digital business operations.

---

### 7️⃣ Cyberwarfare
- The broadest category.
- Involves using information systems to target:
  - Individuals  
  - Organizations  
  - Nations  

Includes:
- **Information terrorism**  
- **Semantic attacks**: Take over systems while making them appear normal  
- **Simula-warfare**: Simulated attacks for influence or intimidation  

---

# 🛡️ Defensive vs Offensive Information Warfare

### **Defensive Information Warfare**
Strategies and actions focused on:
- Prevention  
- Deterrence  
- Alerts  
- Detection  
- Emergency preparedness  
- Response  

Goal: **Protect ICT assets and maintain operational continuity.**

---

### **Offensive Information Warfare**
Actions aimed at attacking an opponent’s ICT assets, including:
- Web application attacks  
- Web server attacks  
- Malware attacks  
- MITM attacks  
- System hacking  

Goal: **Disrupt, compromise, or control enemy systems.**
