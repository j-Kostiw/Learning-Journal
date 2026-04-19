This topic focuses on ensuring ingestion systems are reliable by monitoring performance, predicting issues, and detecting anomalies in real time.

From the session overview :

You are expected to:

Monitor ingestion pipelines
Implement forecasting techniques
Detect anomalies
Integrate monitoring with incident response
Instructor Insight

This topic completes the lifecycle:

Build → Stream → Validate → Monitor → Improve

At EPA level, this demonstrates:

Operational awareness
Reliability engineering mindset
2. Real-World Case Study – Financial Institution

From page 2 :

Full Explanation

A financial system processes high volumes of transactions and needs to:

Detect fraud
Prevent system failures
Techniques Used
Isolation Forest (ML anomaly detection)
Time series models
Streaming integration (Striim)
Outcome
Reduced system issues
Improved efficiency
Enhanced security
Instructor Insight

This is a distinction-level example:

Real-time monitoring → anomaly detection → business protection

KSB Mapping
K2 – Business context
S3 / S5 – Real-time data processing
B1 – Responsible system design
3. Monitoring in Data Engineering (FOUNDATION)

From page 5 :

Full Explanation

Monitoring ensures that data pipelines are functioning correctly, efficiently, and securely.

Why Monitoring is Critical
Ensures data integrity
Maintains system performance
Improves reliability
Supports compliance
Key Monitoring Concepts
Metrics → numerical performance data
Logs → detailed system records
Alerts → notify issues
Dashboards → visualise system state
Instructor Insight

You cannot fix what you cannot see

KSB Mapping
K6 – System performance
S4 – Monitoring systems
B2 – Continuous improvement
4. Industry Tools – Prometheus & Grafana

From page 6 :

Prometheus (Monitoring Engine)
Collects time-series metrics
Uses PromQL for querying
Integrates with Alertmanager
Grafana (Visualisation)
Builds dashboards
Connects to multiple data sources
Provides alerting
Instructor Insight

Prometheus = data collection
Grafana = visualisation

KSB Mapping
K7 / K25 – Tools and platforms
S5 – Implementation
5. Monitoring Kafka Systems

From page 7 :

Full Explanation

Kafka monitoring ensures:

Stable and efficient real-time data pipelines

Key Components
Kafka Exporter → exposes metrics
Prometheus → collects metrics
Grafana → visualises
Key Metrics (CRITICAL)
Broker health
Producer throughput
Consumer lag
Instructor Insight

Consumer lag is one of the most tested concepts in EPA

KSB Mapping
S4 / S5 – Monitoring pipelines
K6 – System behaviour
6. Automating Monitoring (Alerting)

From page 8 :

Full Explanation

Alerting automates detection and response to issues.

Example: Kafka Consumer Lag Alert
Trigger: lag > threshold
Duration: sustained issue
Severity: critical
Key Components
Alert rules
Notification channels
Alertmanager
Instructor Insight

Strong EPA answers include:

Detection + automated response

KSB Mapping
S4 – Monitoring
B2 – Proactive improvement
7. Case Study – Healthcare Pipeline

From page 9 :

Implementation Steps
Deploy Prometheus + Grafana
Configure Kafka exporter
Create dashboards
Define alerts
Integrate incident management
Business Benefits
Improved patient care
Better data integrity
Operational efficiency
Instructor Insight

This shows:

Monitoring → reliability → real-world impact

8. Forecasting in Data Engineering

From page 10 :

Full Explanation

Forecasting predicts future system behaviour using historical data.

Why it matters
Capacity planning
Prevent system overload
Optimise cost
Example (Retail)
Predict demand
Avoid stock issues
KSB Mapping
S3 – Data analysis
K2 – Business impact
9. Time Series Forecasting (CRITICAL)

From page 11 :

Key Concepts
Level → baseline
Trend → direction over time
Seasonality → repeating patterns
Methods You MUST Know
ARIMA
SARIMAX
Prophet
LSTM (advanced)
Instructor Insight

These models are used to predict ingestion rates and detect anomalies

KSB Mapping
K4 / K7 – Data modelling
S3 – Analysis
10. Anomaly Detection Techniques (VERY IMPORTANT)

From page 12 :

Full Explanation

Anomaly detection identifies unusual patterns that may indicate system issues or fraud.

Types of Methods
Statistical
Z-score
Seasonal Hybrid ESD
Machine Learning
Isolation Forest
One-Class SVM
Time Series
ARIMA residuals
Prophet
Instructor Insight

At EPA level:

You should compare approaches and justify usage

KSB Mapping
S3 / S4 – Data analysis and evaluation
K7 – Advanced techniques
11. Integration with Incident Management

From summary (page 15) :

Key Idea

Monitoring systems must connect to tools like PagerDuty for response.

Why it matters
Faster issue resolution
Reduced downtime
Improved reliability
KSB Mapping
S8 – Communication
B2 – Responsibility
12. What Examiners Are Looking For
1. End-to-End Monitoring Thinking

You must describe:

Metrics → Monitoring → Alerting → Response

2. Real-Time Awareness

Explain:

Streaming systems need continuous monitoring
3. Data + System Thinking

Not just:

“Detect anomalies”

But:

“Detect anomalies in ingestion pipelines to prevent system failure and data issues”

4. Tool + Technique Integration

Combine:

Prometheus
Kafka metrics
Forecasting
ML models
13. Final Takeaways

From summary (page 15) :

Monitoring ensures pipeline reliability
Prometheus & Grafana are key tools
Forecasting supports planning
Anomaly detection identifies issues early
Alerting improves responsiveness
Integration with incident tools is critical
14. EPA Revision Checklist

You should be able to:

Explain why monitoring is important
Describe Prometheus & Grafana roles
Identify Kafka metrics (especially lag)
Explain alerting systems
Describe forecasting techniques (ARIMA, SARIMAX)
Compare anomaly detection methods
Link monitoring to business outcomes
15. Final Instructor Insight

A distinction-level apprentice:

Designs systems that don’t just work — they are observable, predictable, and resilient
