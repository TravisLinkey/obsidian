
Tags: [[AWS]] | [[Identity & Federation]]


### Overview

A Web service that allows users to securely control access to AWS resources.

### Types

- [[Users]]: long term credentials
- [[Groups]]
- [[Roles]]: short-term credentials, uses [[STS]]
    - [[EC2 Instance Roles]]: uses the EC2 metadata service. One role at a time per instance
    - [[Service Roles]]: API Gateway, CodeDeploy, etc.[]()
    - [[Cross Account Roles]]

- [[Policies]]
    - AWS Managed
    - Customer Managed
    - Inline Policies

- [[Resource Based Policies]] (S3 bucket, SQS queue, etc.)

### References

