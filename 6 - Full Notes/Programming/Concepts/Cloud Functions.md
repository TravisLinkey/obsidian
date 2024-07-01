
2024-06-08 10:45

Tag: [[Serverless]]

## Overview

Small units of code that execute in response to events. They run in a managed environment where the infrastructure management (server provisioning and scaling) is handled by the cloud provider.

### Key Concepts

- ***Event-driven*** - Triggered by events such as HTTP requests, database changes, file uploads, etc.
- ***Scalable*** - Automatically scale up or down based on the number of incoming requests. 
- ***Managed Environment*** - No need to manage servers, operating systems or runtime environments.
- ***Pay as you go*** - Billed based on actual execution time and resources used, which can be cost-effective for infrequent or sporatic workloads.
- ***Stateless*** - Typically stateless, each function invocation is independent and does not rely on previous invocations.

### Examples
- [[AWS]] [[6 - Full Notes/Programming/Services/Cloud/AWS/Services/Lambda]]
- [[GCP Cloud Functions]]

### Use Cases
- ***Microservices***
- ***Data Processing***
- ***API Backends***
- ***Automation*** - Used for backups, notifications, webhooks, etc
