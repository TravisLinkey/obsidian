
2024-05-29 18:17

Status:
Tag: [[AWS]] | [[6 - Full Notes/Programming/Services/Cloud/AWS/Services/Lambda]]

## Overview
An execution environment in AWS Lambda is a secure and isolated runtime environment that runs your Lambda function code.

## 1. Components:

1. Runtime: Includes the language runtime (Python, Node.js, Java) and dependencies required by your function
2. System Libraries: The libraries required by the runtime and the function code.
3. Lambda Layers: Optional, additional code or libraries that can be included with the function
4. Sandbox: An isolated environment with its own resources, including CPU, memory, and network.

## 2. Lifecycle:

1. Initialization: When a function is invoked for the first time or after being idle, Lambda creates a new execution environment. This includes initializing the runtime and loading the function code.

2. Reuse: After initialization, the environment is kept warm for a period of time to handle subsequent requests. This reduces the latency for subsequent invocations by reusing the existing environment.

3. Shutdown: If an environment remains idle too long, it will shut down to save resources.

## References:
- [AWS Lambda Execution Environment](https://docs.aws.amazon.com/lambda/latest/dg/lambda-runtime-environment.html)
- [AWS Lambda Best Practices](https://docs.aws.amazon.com/lambda/latest/dg/best-practices.html)
