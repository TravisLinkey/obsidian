
Tags: [[IAM]]

### Overview

A service that can help you identify which resources are shared externally.

- [[S3]] buckets
- [[IAM]] [[Roles]]
- [[KMS]] keys
- [[Lambda]] functions and [[Layers]]
- [[SQS]] queues
- [[Secrets Manager]] secrets


### Details

Provides last accessed information data about when AWS services and actions from select AWS services were last used by a role or user through their IAM policies.

Helps you identify opportunities to tighten your permissions.

### Concepts

- Define a [[Zone of Trust]] as an AWS Account or AWS [[Organization]]
- Any access outside of [[Zone of Trust]] will be reported as findings


### Services

- [[Policy Validation]]
- [[Policy Generation]]

