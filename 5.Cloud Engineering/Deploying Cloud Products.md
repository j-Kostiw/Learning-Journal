🧠 Learning Objectives
Understand on-demand cloud release importance.

Practice deploying in the cloud environment.

Evaluate CI/CD best practices.

Explore the DevSecOps toolchain.

🔐 DevSecOps in Action
Activity 1: Developer Conversations
Developer Statement	Secure Response	Why It Matters
“No need for pre-prod environment.”	✅ Recommend adding a pre-prod environment.	Catches real-world integration issues missed in local tests.
“Store API keys in the repo.”	✅ Use GitHub Secrets, Azure Key Vault.	Secrets in source control are vulnerable to leaks.
“Skip security scans for small changes.”	✅ Always scan on every commit.	Vulnerabilities can enter even in small commits.
“No need to scan trusted open-source dependencies.”	✅ Scan always (Snyk, Dependabot).	Even trusted packages can have hidden CVEs (e.g., Log4j).
“Let anyone deploy to prod.”	✅ Restrict with RBAC.	Limits mistakes and malicious access.

🚀 Release Pipelines 101
🔄 Artifact Sources
Build outputs, containers, source control, file shares.

📌 Deployment Considerations
Deployment frequency?

Target environments?

Single vs multi-team use?

Downtime & performance impact?

End-user expectations?

⚙️ Trigger Types
Continuous – auto after build.

Scheduled – e.g., nightly releases.

Manual – human-controlled, good for critical systems.

✅ Release Controls
✋ Manual Approvals
Control whether to release, not how.

Builds trust in automated processes.

🔐 Release Gates (Examples)
No blocker issues.

Code coverage > 80%.

No new vulnerabilities or license violations.

UX performance unaffected.

Linked to specific work items or committer.

📚 GitLab Docs on CI
📚 Azure Release Gates

🏗️ Pipeline Components
🔧 Build & Release Tasks
Modular actions: test, package, deploy.

👷 Jobs
Sequential tasks run on the same target.

Support multi-platform (Windows, Linux, Mac).

📊 Monitoring & Feedback
Release gates, service hooks, and notifications keep stakeholders informed.

🛡️ Security in CI/CD Pipelines
Key Security Practices:
MFA & Just Enough Admin (JEA).

Immutable infrastructure via pipeline-only changes.

RBAC on pipeline permissions.

Dynamic scanning (e.g., penetration tests).

Monitor production for intrusions.

Tools to Know:
Scanning: WhiteSource, Checkmarx, Veracode, Black Duck.

Composition Analysis: Snyk, Clair (image scanning), CVE tracking.

Software Composition Analysis (SCA)
Integrate into pipelines for early detection of known vulnerabilities in dependencies.

🧪 Activity 2: RapidRetail Case Study
🔍 Security Risks Identified:

Risk	Why Risky?	Better Practice
No branch protection	Any user can push to main.	Enforce reviews and protection rules.
Public Docker images	Exposed to external tampering.	Use private registries.
Hardcoded secrets	Easily leaked or exposed.	Store in secret vaults.
No scanning/tests	Vulnerabilities undetected.	Automate scans in the pipeline.
Shared SSH keys	Not auditable or secure.	Use individual credentials with logging.
No monitoring	No detection of runtime issues.	Implement post-deploy monitoring.
No manual approvals	All changes go live.	Use approval gates for validation.

🧬 DevSecOps Overview
Definition:
A blend of DevOps and security practices to build fast, secure systems.

Goals:

Automate security early in the SDLC.

Maintain velocity without compromising safety.

Transition Steps:

Secure pipeline stages (build, test, release, deploy).

Automate compliance and validation.

Encourage collaboration between security, dev, and ops.

🔄 CI/CD Pipeline Breakdown
Build – Compile code.

Test – Run automated unit & integration tests.

Release – Package and store artifacts.

Deploy – Push to target environment.

Validation – Check for CVEs, quality, compliance.

🛠️ Tool highlight: Clair by Red Hat

[L5DE M5T4 Webinar.pdf](https://github.com/user-attachments/files/21428203/L5DE.M5T4.Webinar.pdf)
