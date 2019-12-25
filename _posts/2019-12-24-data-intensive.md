---
title: Data Intensive Applications
layout: post
---

## Humble beginnings

For a long time it has been somewhat of a mystery how large companies like Amazon ot Netflix are able to manage the complexity of their systems. At such a masive scale, even a few minutes of downtime can cause chaos where payments might be missed leading to inconsistent state in the database (and a bunch of angry customers to follow). Therefore, I have decided to take on the task to remove the mystery surrounding such massive systems and as a part of this journey I read a book called Designing Data Intensive Applications by Martin Kleppmann. The book touches on a wide range of the most important topics in distributed systems from which it becomes possible to dive even deeper into specific technologies or research topics. I really enjoyed the book, and to distill the most important topics for myself for future reference I wanted to write a bit about the most important lessons I had learned while reading this masterpiece.

## Types of Databases

### Relational
The most commonly used data model is probably the Relational model, where data is stored in relations (aka tables in SQL) where each relation is an unordered collection of tuples (rows in SQL). A RDMS is often highly optimized to perform joins between tables and allows users to create key-based relations between tables. Relational schemas are very explicit and inflexible, and to make a change to the schema a migration must be performed. 

### Document-oriented
Instead of storing an application's data in a very structured way such as in a relational database it is also possible to use a document. Usually, a document is of a standardized format (but not schema) such as JSON, XML, YML or BSON (MongoDB). The database retains keys that map to each document, where keys can be a path or some unique ID. Documents usually don't have a predefined schema and it is up to the application where the schema is validated.

<!-- ### Wide-column -->
### Graph-based 
Some data can best be modeled as a set of many-to-many relations, in such cases a graph-like data model might be best. Such databases usually have a query language that is optimized to perform operations on graphs, such as calculating the page rank, or some other metric of a vertex. The same could in theory also be done in SQL, but tends to be unnecessarily complicated.

## Flavours of databases
The book describes two main approaches to building highly peformant databases, Sorted Strings Table (SSTable) and an Log-Structured Merge Tree

## The internals of indices

## Isolation

## Linearizations vs Serializability

## Write Skews and Phantoms

## Message Brokers

## ACID

## CAP

