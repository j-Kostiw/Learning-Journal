🔄 Migration Types
Type	Description
Rehosting (Lift & Shift)	Move as-is, no code changes.
Refactoring	Modify app for cloud-native benefits.
Rebuilding	Start from scratch, full redesign.

✅ Success Factors
Assess readiness and cloud fit.

Plan data transfer and integration carefully.

Train staff and manage cultural change.

📉 Common Pitfalls
Vague objectives.

Underestimating costs or time.

Ignoring internal resistance.

Lack of training.

📚 Case Studies
✅ Capital One: Cloud-first approach led to faster innovation & better security.
❌ Target: Migration failed due to underestimated complexity, lack of expertise, and cultural resistance.

🗄️ Cloud Archiving
📌 Why Archive?
Compliance with regulations (e.g., GDPR, HIPAA).

Preserve historical data.

Reduce load on primary storage.

🧱 Policy Essentials
Data Classification: What's archival-worthy?

Retention Schedules: How long to keep?

Access Controls: Who gets access?

Disposal Procedures: Secure data deletion.

🌡️ Storage Tiers
Tier	Use Case
Hot	Frequently accessed data.
Cold	Rarely accessed, low-cost (e.g., Amazon Glacier).

✅ Best Practices
Deduplicate and compress data.

Encrypt data with secure key management.

Run regular audits and policy reviews.

⚠️ Challenges & Solutions
Challenge	Solution
Legacy Formats	Migrate to modern standards.
Rising Costs	Use cold storage tiers strategically.

🔍 Monitoring & 🛡️ Disaster Recovery
🧭 Why Monitoring Matters
Early warning of issues (e.g., CPU spikes, failed jobs).

Enables proactive fixes before users are affected.

🧰 Tools
Azure Monitor

CloudWatch

Grafana (for dashboards)

🛠️ DR Plan Components
Element	Purpose
Risk Assessment	Identify threats.
Business Impact Analysis	Set priorities and RTO/RPO.
Recovery Strategies	Describe how to restore systems.
Comms Plan	Keep stakeholders informed.

🔁 Redundancy Types
Type	Description
Data	Multiple copies stored.
Hardware	Backup servers/devices.
Network	Multiple paths to avoid outages.

🧪 Labs
🧬 Option 1: Amazon EMR Log Processing
Use Apache Hive on EMR to process logs in S3.

Focus: Big data pipelines with cloud-native tools.

Time: ~90 mins

🍽️ Option 2: DynamoDB Menu Management
Build a menu system with Amazon DynamoDB.

Learn querying, indexing, and structured NoSQL storage.

Time: ~90 mins

📚 Post-Webinar Tasks
Write a Migration Plan
Include risks and lessons from real-world failures.

Draft a DR Plan
Include incident response steps and communication paths.

Audit Your Monitoring
Review your company’s setup, or prototype a custom dashboard.

Extra Practice

AWS Cloud Foundations – Module 7

Lab 4 – Working with EBS

🧠 Final Takeaways
Migrations, archiving, monitoring, and DR are core to cloud resilience.

Well-designed archiving policies = lower cost, legal compliance.

The Power/Interest Matrix helps align cloud strategies with stakeholders.

Redundancy ensures uptime and reliability.

DR & Monitoring strategies must be planned, tested, and automated.

[Level 5 Data Engineer Module 5 Topic 5 - Migrations, archiving, monitoring, and disaster recovery.pdf](https://github.com/user-attachments/files/21428272/Level.5.Data.Engineer.Module.5.Topic.5.-.Migrations.archiving.monitoring.and.disaster.recovery.pdf)
