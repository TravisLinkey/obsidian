
2024-06-08 21:24

Tag: [[3 - Tags/ADR|ADR]] | [[System Design]]

## Overview

Current project we need to make a decision whether we want our core application to be lambdas or containers.

Here is what I think and why:

### Decision

I believe we should refactor our application to run on containers.

### Reasoning - High level

- Cold Start times
- Long running process (Websocket communication)
- Local testing (Local stack)
- Monorepo - Use docker-compose to run multiple applications (Salesperson FE, BFF, Transaction Process, Elavon Service, Email Service)

## References:
- [[6 - Full Notes/Deep Dives/Containers vs. Lambdas|Containers vs. Lambdas]]

