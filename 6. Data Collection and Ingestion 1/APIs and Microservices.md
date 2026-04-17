How data engineers use APIs and microservices to collect, move, and scale data systems

This is about:

Integrating systems
Scaling pipelines
Designing modern architectures
2. Key Concepts from Slides
What is an API?

From diagram (page 8) :

Simple definition:

An API allows systems to communicate and exchange data

Flow (from diagram):
Client sends request
Server routes to API
API interacts with database
Data returned
Response sent to client
EPA Insight:

APIs are data access layers, not storage systems

REST APIs (Very Important)

From page 9 :

Key components:
HTTP methods:
GET → retrieve data
POST → create
PUT → update
DELETE → remove
URL endpoints
JSON responses
Example:
GET /users/123
Why REST matters:
Standardised
Scalable
Widely used in data ingestion
Using APIs for Data Ingestion

From objectives (page 5) :

Key idea:

APIs allow you to pull data from external systems into pipelines

Example:
Pulling data from:
Government APIs
Social media
Third-party services
KSB Mapping
S2 / S5 – Building ingestion pipelines
K4 – Data integration
3. Microservices Architecture
What are Microservices?

From case study (page 3) :

A system made up of independent services that communicate via APIs

Key Benefits (Exam Critical)

From knowledge check (page 4) :

Main benefit:

Independent scaling and deployment

Full benefits:
Scalability
Flexibility
Fault tolerance
Faster deployment
Netflix Case Study (Strong Example)

From page 3 :

Architecture:
Separate services:
Authentication
Recommendations
Streaming
Why it works:
Each service can scale independently
Failures don’t break the whole system
EPA Insight:

Monolithic vs microservices comparison is a strong discussion point

4. API + Microservices in Data Engineering
How they work together:
APIs = communication layer
Microservices = architecture
Example pipeline:
API collects data
Microservice processes it
Another service stores it
Designing Ingestion Architectures

From summary (page 30) :

Good design includes:
Modular services
Scalable ingestion
Real-time capability
EPA Tip:

Always describe:

“How components interact”

5. Python API Integration (Practical Skills)
Using requests

From page 12 :

Core usage:
import requests
r = requests.get("https://api.github.com/events")
Key points:
Send HTTP requests
Receive JSON data
Handle authentication
Handling Responses

From pages 13–14 :

Status code categories:
2xx → success
4xx → client error
5xx → server error
Example:
200 → OK
404 → Not found
500 → server error
EPA Insight:

Always check response codes before processing data

Error Handling (Critical Skill)

From pages 15–21 :

Use try/except:
try:
    response = requests.get(url)
except:
    print("Error occurred")
Advanced:
Multiple exceptions
Finally block (cleanup)
Raise errors
Why this matters:
APIs fail frequently
Robust pipelines require error handling
KSB Mapping
S2 / S5 – Reliable pipelines
B2 – Professional coding practices
6. API Security & Access Control
OAuth (Page 28)

Purpose:
Secure API access
Authorisation (who can access what)
How it works:
User authenticates
Receives token
Token used for API calls
API Gateways

From page 28 :

Role:
Central entry point
Handles authentication
Routes requests
JWT (Page 29)
Purpose:
Secure data exchange
Token-based authentication
Why this matters (EPA Insight):

Data engineers must consider:

Security
Access control
Compliance
7. API Aggregators

From page 26 :

Definition:

Combine multiple APIs into one interface

Benefits:
Simplifies integration
Reduces complexity
Improves consistency
Example:
Tools like Zapier
8. Practical Architecture Thinking
When designing systems:

You must consider:

Data sources (APIs)
Processing (microservices)
Storage (databases)
Access (dashboards/APIs)
9. What Examiners Are Looking For
1. Clear Understanding of APIs

Not just:

“APIs get data”

But:

“APIs provide structured, secure access to external data sources using HTTP protocols”

2. Architecture Thinking

Explain:

Components
Interactions
Benefits
3. Scalability Awareness

Microservices should always link to:

Scaling
Fault tolerance
4. Practical Awareness

Mention:

requests library
JSON
Error handling
10. Final Takeaways

From summary (page 30) :

Microservices enable scalability and flexibility
APIs enable efficient data ingestion
Combined architecture improves performance
11. EPA Revision Checklist

You should be able to:

Explain what an API is and how it works
Describe REST APIs and HTTP methods
Explain microservices architecture
Justify why microservices improve scalability
Show how APIs are used in ingestion pipelines
Demonstrate error handling in API calls
Discuss security (OAuth, tokens, gateways)
