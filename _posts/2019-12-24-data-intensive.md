---
title: Takeaways from Designing Data Intensive Applications
layout: post
---

## Humble beginnings

For a long time it has been somewhat of a mystery how large companies like Amazon ot Netflix are able to manage the complexity of their systems. At such a masive scale, even a few minutes of downtime can cause chaos where payments might be missed leading to inconsistent state in the database (and a bunch of angry customers to follow). Therefore, I have decided to take on the task to remove the mystery surrounding such massive systems and as a part of this journey I read a book called Designing Data Intensive Applications by Martin Kleppmann. The book touches on a wide range of the most important topics in distributed systems from which it becomes possible to dive even deeper into specific technologies or research topics. I really enjoyed the book, and to distill the most important topics for myself for future reference I wanted to write a bit about the most important lessons I had learned while reading this masterwork.

## Types of Databases
### Document-oriented
### Relational
### Wide-column
### Graph-based 

## Flavours of databases
The book describes two main approaches to building highly peformant databases, Sorted Strings Table (SSTable) and an Log-Structured Merge Tree

## The internals of indices

## Isolation

## Linearizations vs Serializability

## Write Skews and Phantoms

## Message Brokers

## ACID

## CAP

