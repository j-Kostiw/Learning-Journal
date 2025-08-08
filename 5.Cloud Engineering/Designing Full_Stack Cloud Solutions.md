🔄 DevOps Loop: "Inner Loop" of a Sprint
This loop happens within a development sprint:

Code

Build

Test

Think of this as your daily grind — where fast iteration happens before pushing to wider environments.

📊 Monitoring in Azure
🧭 Azure Monitor (Unified Tool)
Previously separate tools (Log Analytics + Application Insights) are now under Azure Monitor.

Use Azure Monitor to:

Track performance of web apps

Diagnose problems

Set up alerts

Visualise metrics and logs

🔍 Log Analytics + KQL
Log Analytics lets you query logs for insights.

KQL (Kusto Query Language) is how you write those queries.

Resource: Learn KQL here

💡 Why learn KQL?
It’s powerful for filtering, analyzing, and visualizing large log datasets across many Azure services.

🧪 Monitoring in Practice: The Lab
You'll practice:

Deploying a web app on Azure App Service

Adding Application Insights

Monitoring traffic, performance, and usage

Creating alerts and investigating issues

📈 Monitoring Application Performance
Why does this matter?

1. Monitor – Stay aware of how your app is running
2. Detect & Diagnose – Catch bugs or slowdowns early
3. Build, Measure, Learn – Use feedback to improve continuously

🛠️ Tools You’ll Use
🔧 App Center Diagnostics
Tracks crashes and app health

Captures the state before a crash

Sends alerts (email) when new crash groups happen

📌 Think of this as your "black box recorder" for apps.

🐞 Bug Tracking
Set up alerts to auto-create bugs when issues arise. It helps keep response times quick and systematic.

📊 Dashboards & Visual Tools
Azure Dashboards – Summary views for your resources.

View Designer / Workbooks – Build custom data visualizations.

Grafana – Advanced, open-source tool to combine data from multiple sources.

🛠️ Build Your Own Monitoring Tool?
You could — but be cautious:

✅ Pros: Full flexibility
❌ Cons: High engineering effort needed (not beginner-friendly)

✅ Quick Recap Questions (Check your understanding)
What are the advantages of using Azure Monitor over separate tools?

Why is KQL useful in a monitoring context?

What steps are involved in setting up App Center crash alerts?

What’s the difference between using dashboards vs. building a custom monitoring tool?

How does monitoring support sustainability in cloud engineering?
[Uploading L5DE M5T7 Webinar.pdf…]()
