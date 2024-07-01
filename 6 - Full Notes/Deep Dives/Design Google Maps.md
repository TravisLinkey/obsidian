

2024-06-06 18:53

Status:
Tag: [[Deep Dive]] | [[System Design]]

## Overview

A physical location is translated into a coordinate (longitude, latitude). A data structure is used to index and query for these coordinate points. ([[Quadtree]])

A graph database is used to represent the possible paths between the source and destination. This graph uses [[Spatial Indexing]]  to find and traverse the tiles in the graph. We can apply a search algorithm, (possibly [[Djikstra's]]) to find the shortest path.

## Architecture

![[Design Google Maps.png]]

#### Client

The client could use two-way communication ([[Web Sockets]]) with the Location Service for real time updates.

#### Route Service

Used to return the shortest route to the user. 

The route data would be stored in a [[Graph Database]]. This database could be optimized with [[Sharding]] using the first few digits of a [[Geohash]]. (Similar, close together shards are grouped together in a shard)

The cache could contain the [[Quadtree]] of [[Spatial Indexing]] indices. Or possibly commonly visited routes.

#### Location Service

Used to track traffic conditions. This can affect the shortest route.

This will need to call a NoSQL database that can withstand heavy write traffic (time-series data) for historical data on user locations and which roads / routes have how much traffic at any point in time. A good solution would be [[Cassandra]].

In reality, we would not want to read the data from the NoSQL database directly, instead it would use a [[Message Queue]] or [[Streaming Service]] like [[Kafka]] or [[Kinesis]]

#### CDN

We also want to support pictures of the routes themselves (for the UI). This can be done using a [[CDN]] and an [[Object Store]].

To properly index the images in the CDN, we can encode the image url with the routes [[Geohash]] for quick retrieval.

## References:

[Neetcode IO](https://neetcode.io/courses/system-design-interview/7)