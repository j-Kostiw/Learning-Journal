Cybersecurity Architecture Phases: likely involve Planning, Implementation, and Monitoring.

5 Rules of Networking: Secure communication, identity management, access controls, visibility, and resilience.

Zero Trust: "Implicit trust is never assumed—always verified."

🔍 Remember: Authentication ≠ Authorization

Authentication = who you are

Authorization = what you’re allowed to do

🧱 Secure by Design
Integrate security from the start (not patched later).

Key benefits: lower long-term costs, better trust, resilient systems.

Analogy: Like building a house with reinforced locks and alarms, not installing them after a break-in.

📖 Essential Concepts & Terms
Service / Service Account: Used to manage system-to-system authentication.

Externally-exposed Assets: Require extra hardening.

Threat Modelling: Identify, assess, and prioritize security threats.

Redundancy & Resilience: Design to recover and continue under failure.

Security Controls: Tools, policies, and measures that reduce risk.

🔐 Security Control Frameworks
Set the standards and expectations for secure systems.

Comparable to building codes in architecture.

🧩 Design Principles for Secure Architecture
Key Patterns:
Principle	Description	Benefit
Least Privilege	Only necessary access	Limits damage from breaches
Defense in Depth	Multi-layered security	Redundant protection
Economy of Mechanism	Keep it simple	Fewer errors, easier audits
Fail-Safe Defaults	Deny by default	Reduces attack surfaces
Complete Mediation	Validate every access	Prevents privilege creep
Open Design	Don’t hide mechanisms	Encourages peer-reviewed security
Separation of Privilege	Dual control for sensitive actions	Limits insider threats
Least Common Mechanism	Avoid shared services	Reduces inter-user leaks
Psychological Acceptability	User-friendly security	Encourages compliance

⚠️ Common Anti-Patterns
Avoid these mistakes:

Security by Obscurity (e.g. hiding code logic).

Poor default configurations.

Overly permissive access.

🛡️ Practical Security Techniques
Technique	Example
Secure Communication	TLS/SSL for DB to cloud
Secure Config	Disable root login, remove unused services
Access Control	IAM roles + MFA
Monitoring & Logging	CloudTrail with alerts to SIEM
Patch Management	Automate critical vulnerability updates

🔒 Secure Protocols & Infrastructure
Key Protocols:
SSL/TLS: Encrypt data in transit.

HTTPS: HTTP + SSL/TLS.

VPNs: Secure remote connections.

X.509 Certificates: Identity verification in SSL.

Best Practices:

Use latest protocol versions.

Enable Perfect Forward Secrecy.

Avoid downgrade attacks (mitigate with TLS_FALLBACK_SCSV).

🧨 OWASP Top 5 Vulnerabilities
Broken Access Control: Missing permission checks.

Cryptographic Failures: Weak/no encryption.

Injection: SQL, XML, etc. from unvalidated inputs.

Insecure Design: Overexposed diagnostics/logging.

Security Misconfiguration: Default settings, unpatched software.

💡 Example: SQL Injection—' OR 1=1 -- turns queries into backdoors.

[Level 5 Data Engineer Module 4 Topic 3 - Designing secure architectures.pdf](https://github.com/user-attachments/files/20834737/Level.5.Data.Engineer.Module.4.Topic.3.-.Designing.secure.architectures.pdf)
