
2024-06-07 21:30

Tag: [[System Design]] | [[Event Driven]]

## Overview

Publish-Subscribe Model is a messaging pattern where messages are published to a topic by a publisher and are received by one or more subscribers.

The key characteristic of this model is the decoupling of publishers and subscribers, which allows for scalability and flexibility in the design of [[Distributed Systems]].


### Key Concepts:

- **Publisher** - an entity that sends messages to a topic
- **Subscriber** - an entity that receives messages from a topic.
- **Topic** - A named channel to which publishers send messages and from which subscribers receive messages.
- **Message** - Data or information sent from the publisher to the subscriber via the topic.

### Example Architectures

#### AWS - [[SNS]]

1. Publisher: An e-commerce application generates order events.
2. Subscriber: 
	1. An email service that sends order confirmation emails.
	2. A warehouse management system that processes order for shipments.

#### GCP - [[Google Cloud Pub-Sub]]

1. Publisher: A sensor network that collects environmental data.
2. Subscribers:
	1. Data processing service that analyzes the sensor data.
	2. Storage service that archives the raw sensor data.

## References:

[Wiki Link](https://en.wikipedia.org/wiki/Publish%E2%80%93subscribe_pattern)