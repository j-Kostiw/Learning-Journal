[L5DE M3T9 V1.pdf](https://github.com/user-attachments/files/20408991/L5DE.M3T9.V1.pdf)

Key Concepts

Modern data engineering systems require:

reliable deployments,
automated testing,
scalable infrastructure,
operational monitoring,
and rapid recovery from failure.

DevOps pipelines support this through:

Continuous Integration (CI),
Continuous Delivery (CD),
Continuous Deployment.
DevOps Pipeline Lifecycle

The DevOps lifecycle was structured as:

Stage	Purpose
Code	Continuous Integration
Build	Continuous Delivery
Release	Continuous Deployment

This structure enables:

repeatable deployments,
operational consistency,
faster issue detection,
reliable releases.
Benefits of DevOps Pipelines

Benefits introduced included:

reduced risk,
shorter review times,
better code quality,
faster bug fixes,
measurable progress,
rapid feedback loops,
increased collaboration.
Continuous Integration (CI)

CI focuses on:

frequent code merging,
automated testing,
build validation,
early issue detection.

Typical workflow:

Run tests locally
Compile mainline
Run tests on mainline
Report on tests.
CI Best Practices

Key practices included:

maintaining a code repository,
automating builds,
self-testing,
committing daily,
building every commit,
ensuring every bug has a test.

These practices improve:

software reliability,
deployment quality,
operational stability.
CI Monitoring and Visibility

CI provides operational visibility through:

automated reporting,
build status tracking,
static analysis,
test metrics,
failure alerts.

This enables rapid identification of:

broken builds,
failing tests,
integration issues.
Continuous Delivery (CD)

Continuous Delivery ensures:

software is always potentially releasable,
builds remain tested,
deployment candidates are validated continuously.

Benefits:

faster releases,
improved product quality,
reduced release risk,
higher customer satisfaction.
Continuous Deployment

Continuous Deployment automates production releases without requiring manual approval.

Benefits:

faster delivery,
quicker bug resolution,
reduced deployment delays.

Trade-off:

requires extremely reliable testing and monitoring.
K3 — Data Normalisation Principles

KSB:
Data normalisation principles and the advantages they achieve in databases for data protection, redundancy, and inconsistent dependency.

Key Concepts

Although the topic focused primarily on DevOps and deployment engineering, structured development practices still support:

consistency,
maintainability,
modular system design,
predictable integration behaviour.
Consistent Environments

Containerisation helps ensure:

applications behave consistently,
dependencies remain controlled,
environments are reproducible.

This reduces:

environment drift,
inconsistent deployment behaviour,
integration inconsistencies.
Infrastructure Standardisation

Infrastructure as Code (IaC) treats infrastructure like software code:

version-controlled,
repeatable,
configurable,
automated.

This supports:

consistency,
governance,
deployment standardisation.
Modular System Design

Containers promote modular architecture by packaging:

code,
libraries,
runtime environments,
dependencies,
operating system components.

This improves:

portability,
maintainability,
deployment consistency.
K5 — Risks, Ethics and Data Quality

KSB:
The inherent risks of data such as incomplete data, ethical data sources and how to ensure data quality.

Key Concepts

Poor deployment processes introduce risks such as:

unstable releases,
production failures,
broken pipelines,
inconsistent environments,
insecure deployments.

DevOps practices reduce these risks through:

automation,
testing,
reproducibility,
controlled deployment pipelines.
Testing and Quality Assurance

CI emphasises:

automated testing,
self-testing systems,
validating every commit,
detecting issues early.

Benefits:

fewer production defects,
reduced operational failures,
improved reliability.
Risks of Poor Testing

Disadvantages highlighted included:

tests are time-consuming to create,
pipeline value depends on test quality,
some systems are difficult to automate.

This reinforces the importance of:

robust testing strategy,
reliable validation,
continuous quality monitoring.
Deployment Risk Reduction

Continuous Delivery reduces risk through:

shorter release cycles,
continuous validation,
rapid feedback loops,
automated deployment preparation.
Environment Isolation

Containers isolate applications from host systems.

Benefits:

reduced dependency conflicts,
safer deployments,
predictable runtime behaviour.
K18 — Streaming, Batch and On-Demand Data Movement

KSB:
How to use streaming, batching and on-demand services to move data from one location to another.

Key Concepts

DevOps and containerisation are foundational for modern data pipelines because they support:

scalable processing,
automated deployment,
distributed execution,
operational consistency.
Data Pipelines

The practical walkthrough focused on building a pipeline that:

follows programming best practices,
processes data,
generates visualisation outputs.
Deployment Pipelines

Continuous Delivery pipelines automate:

building,
testing,
deployment,
release preparation.

This improves:

operational efficiency,
scalability,
repeatability.
Containers in Data Engineering

Containers support:

portable pipeline execution,
cloud-native workloads,
scalable ingestion systems,
reproducible environments.

Key characteristics:

lightweight,
isolated,
OS agnostic,
“write once, run anywhere.”
Kubernetes and Orchestration

Kubernetes was introduced as a container orchestration platform.

Its primary role:

automating management of containerised applications.

Key features:

scalability,
resource management,
API-driven automation,
workload orchestration.
Docker

Docker simplifies:

environment setup,
rapid deployment,
code distribution,
collaboration.

This is highly valuable in:

distributed engineering teams,
cloud-native data systems,
CI/CD pipelines.
K27 — Descriptive, Predictive and Prescriptive Analytics

KSB:
The principles of descriptive, predictive and prescriptive analytics.

Key Concepts

Analytics systems depend on:

reliable deployments,
scalable infrastructure,
reproducible environments,
automated testing.
Production-Ready Analytics Pipelines

The module emphasised preparing code for production through:

DevOps pipelines,
testing,
deployment automation,
infrastructure management.

This is critical because analytics systems must:

remain available,
scale under load,
produce reliable outputs.
Data Visualisation Pipeline

The practical walkthrough demonstrated building a pipeline that:

processes data,
applies programming best practices,
produces visualisation outputs.

This reflects real analytics engineering workflows.

Faster Feedback Loops

CI/CD improves analytics development through:

continuous testing,
rapid iteration,
shorter deployment cycles,
immediate feedback on changes.
S7 — Working with SQL, NoSQL and Distributed Data Stores

KSB:
Work with different types of data stores, such as SQL, NoSQL, and distributed file system.

Key Concepts

While this topic focused mainly on software engineering and deployment practices, several technologies support distributed data engineering environments.

Containers and Distributed Systems

Containers package:

application code,
dependencies,
runtime environments,
supporting libraries.

This supports:

distributed applications,
scalable deployment,
cloud-native platforms.
Kubernetes Architecture

Kubernetes enables:

distributed workload management,
container orchestration,
scaling across clusters.

This is critical for:

large-scale data platforms,
distributed analytics systems,
scalable ingestion pipelines.
Docker vs Kubernetes

Comparison highlights:

Docker	Kubernetes
Isolation	Scalability
Resource control	API-driven
Container runtime	Orchestration
Simpler setup	Higher complexity

S15 — Optimising Data Ingestion

KSB:
Optimise data ingestion processes using batch, streaming and on-demand frameworks.

Key Concepts

CI/CD and containerisation improve ingestion systems through:

automation,
repeatability,
scalability,
reliable deployment.
Automated Pipeline Deployment

CI/CD pipelines automate:

builds,
testing,
release preparation,
deployment validation.

This reduces:

manual errors,
inconsistent environments,
operational delays.
Infrastructure as Code (IaC)

IaC improves ingestion deployment by allowing infrastructure to be:

version controlled,
reproducible,
automatically provisioned.

Benefits:

speed,
cost reduction,
lower operational risk.
Scalability Through Containers

Containers improve ingestion scalability because they are:

lightweight,
rapidly deployable,
isolated,
portable.
Automated Testing in Pipelines

Pipeline quality depends heavily on:

automated tests,
integration testing,
reproducible builds,
deployment validation.

This ensures ingestion pipelines remain:

stable,
reliable,
production-ready.
Overall Understanding

Modern data engineering requires strong software engineering and DevOps practices alongside technical data skills.

Key areas include:

CI/CD pipelines,
automated testing,
containerisation,
infrastructure automation,
deployment orchestration,
scalable environments,
and production readiness.

Data engineers are increasingly responsible for:

building deployable systems,
automating infrastructure,
managing scalable environments,
monitoring operational reliability,
and ensuring secure, repeatable deployments.

The overall goal is to deliver:

reliable data products,
scalable pipelines,
resilient infrastructure,
and production-quality analytics systems.
