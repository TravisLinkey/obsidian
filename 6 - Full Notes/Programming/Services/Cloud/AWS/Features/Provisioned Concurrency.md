
2024-05-29 18:08

Status:
Tag: [[AWS]] | [[6 - Full Notes/Programming/Services/Cloud/AWS/Services/Lambda]]

## Overview
Provisioned Concurrency is a feature of AWS Lambda that ensures that a Lambda function is prepared to handle requests with predictable latency.

When you enable Provisioned Concurrency, AWS Lambda initializes a requested number of execution environments and keeps them running to be immediately available to respond to invocations.

This helps to reduce the cold start latency that can occur when functions are invoked after being idle.

## Considerations
1. Cost - Provisioned Concurrency incurs additional costs that you are paying for the pre-initialized environments, even if they are not handling requests.

## References:
- [AWS Docs](https://docs.aws.amazon.com/lambda/latest/dg/configuration-concurrency.html)
- [Managing Provisioned Concurrency](https://aws.amazon.com/blogs/compute/new-for-aws-lambda-predictable-start-up-times-with-provisioned-concurrency/)

