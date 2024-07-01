
2024-06-08 13:21

Tag: [[AWS]] | [[System Design]] | [[Streaming Service]]

## Overview

|  | Kinesis Data Streams | Amazon Data Firehose |
| --------------- | --------------- | --------------- |
| Purpose | Low latency streaming service for ingest at scale | Data transfer service to load streaming data into [[S3]], [[Redshift]], [[OpenSearch]] or other third-party tools |
| Message propagation delay | Real time (~200 ms latency for classic shared throughput and ~70ms for enhanced fan out) | Near real time (depends on the buffer size OR buffer time with min. 60 secs) |
| Provisioning | Managed service but needs configuration for shards | Fully managed service with no administration |
| Scaling | Manual scaling | Automated scaling - as per the demand |
| Data storage | Configurable from 1 day to 365 days | Does not provide data storage |
| Replay capability | Supported | Not supported |
| Producers | Next to write code for producers. Supports SDK, KPL, Kinesis Agent, CloudWatch, IoT | Need to write code for producer. Supports SDK, KPL, Kinesis Agent, CloudWatch, IoT |
| Consumers | Open ended. Supports multiple consumers and destinations. Supports KCL and Spark | Close ended. Handled by Firehose and supports limited destinations. Does not support KCL or Spark. |

## Purpose

- [[Kinesis Data Streams]] - A highly customizable and best suited for developers building custom applications or streaming data for specialized needs.
- [[Amazon Data Firehose]] - Handles loading data streams directly into AWS products for processing. Firehose also allows for streaming to [[S3]], [[OpenSearch]], or [[Redshift]], where data can be copied for processing through additional services.

