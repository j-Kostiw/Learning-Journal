🔐 1. CIA Triad
Principle	Goal	Key Techniques
Confidentiality	Prevent unauthorized access to data	Encryption, Access Controls, Authentication
Integrity	Ensure data is unaltered and trustworthy	Hashing, Digital Signatures
Availability	Ensure data/services are accessible when needed	Backups, Redundancy, Load Balancing

🔑 2. Encryption & Cryptography
🔒 Symmetric Encryption
One shared key for encryption and decryption.

Fast, suitable for VPNs.

Examples: AES, DES

Types: Block ciphers (fixed-size chunks) and stream ciphers (bit-by-bit).

🔓 Asymmetric Encryption
Public key + Private key pair.

Slower, used for secure key exchange and digital signatures.

Examples: RSA, ECC

Use Cases:

Alice encrypts with Bob’s public key → only Bob can decrypt with private key → confidentiality.

Alice signs with her private key → anyone can verify with her public key → authentication.

🛡️ 3. Hashing & Integrity
📎 Hash Functions
Converts data into a fixed-length digital fingerprint.

One-way function (cannot reverse easily).

Used to ensure data hasn’t been tampered with.

Popular Hashing Algorithms
Algorithm	Digest Size	Notes
MD5	128-bit	Obsolete, vulnerable
SHA-1	160-bit	Obsolete, vulnerable
SHA-2	256, 384, 512-bit	Recommended
SHA-3	Modern alternative	Preferred for new systems

🔐 4. Public Key Infrastructure (PKI)
Digital Certificates & Trust
Digital Certificate: Binds public key to an entity (e.g., website).

Certificate Authority (CA): Issues certificates (like a trusted passport office).

Registration Authority (RA): Verifies identity on behalf of CA.

PKI Functions
Manage key pairs (public/private)

Issue, revoke, and validate certificates

Foundation of secure websites (HTTPS) and digital signatures

🔏 5. Digital Signatures
How It Works:
Data is hashed.

Hash is encrypted with sender’s private key.

Recipient decrypts hash with sender’s public key.

If hashes match → data is authentic and untampered.

Use Cases:
Code signing

Email signing

Software distribution

🧰 6. Access Control & AAA
Authentication, Authorization, Accounting (AAA)
Term	Purpose
Authentication	Verify identity (e.g., password, biometrics)
Authorization	Define access rights (who can do what)
Accounting	Record activities for auditing and billing

🧮 7. Risk Management & NIST Framework
NIST Cybersecurity Framework – 5 Functions
Function	Description
Identify	Know what needs protecting
Protect	Implement security controls
Detect	Monitor for threats
Respond	Take action when attacked
Recover	Restore operations post-attack

⚖️ 8. Binary Risk Assessment
Quick 4-Step Process:
Identify assets (e.g., databases, APIs).

Identify threats (e.g., phishing, ransomware).

Assess risk (Yes/No).

Implement controls (firewalls, backups, training).

Benefits:
Simple, fast decision-making

Good for triaging smaller risks

💸 9. Financial Impact Analysis
Key Metrics:
Metric	Description
SLE	Single Loss Expectancy (£ per incident)
ARO	Annual Rate of Occurrence
ALE	Annual Loss Expectancy = SLE × ARO

ROI on Controls:
ROI = (ALE_before – ALE_after) / Cost of control

Helps justify security investments (e.g., anti-phishing tools)

🧪 10. Practical Activities & Labs
Hands-On Practice:
AES encryption/decryption: encode-decode.com

Browser certificate inspection

Binary risk analysis: binary.protect.io

📝 Revision Questions
What does the CIA Triad stand for?

What’s the difference between symmetric and asymmetric encryption?

What is ALE and how is it calculated?

How does a digital signature ensure authenticity?

What are the 5 NIST Framework functions?

📚 Recommended Resources
Tools
SIEM Systems: Real-time monitoring

IDS/IPS: Intrusion detection/prevention

Encryption Tools: OpenSSL, GPG

Certifications
CISSP (Certified Information Systems Security Professional)

CEH (Certified Ethical Hacker)

Standards
NIST Cybersecurity Framework
ISO 27001

[Level 5 Data Engineer Module 4 Topic 2 - Cyber Security.pdf](https://github.com/user-attachments/files/20625899/Level.5.Data.Engineer.Module.4.Topic.2.-.Cyber.Security.pdf)



