---
layout: post
title: "Semantic Relationships"
date: 2016-10-25
---

It has been a while since I have worked on backend design and development. My recent projects already have its database implementation, and I just need to create wrappers or services as a middleware that connects the client and the server application. Most of these projects used the good old RDBMS (SQL-based) as the backend. Because of this, I have been itching to learn something new, specifically on the latest data persistence technologies.

One of my goals this month is to research on databases that will suit my use cases for my personal/hobby project - something that supports data model based on _domain-driven design_ with multiple nested relationships, that can result to very complex queries. I have learned that if I have a complex, join-intensive queries, or path-finding queries, then using graph database like Neo4J will be the best option.

In a __graph database management system__, the ‘join’ operations are pre-calculated and explicitly persisted in the database based on the relationships that connect nodes together, simplifying joins like hopping from one node to another. 

Here are some of the concepts that I have learned today about Graph DB (Neo4J)

### Labeled Property Graph (LPG)
This is one of the most generic and versatile of all graph models, and this is the underlying data model of Neo4j.

### Data Constructs
* __Nodes__ - these are typically used to store entity information.
* __Relationships__ - these are used to connect nodes to one another explicitly, providing a way of structuring your entities. These are the equivalent of stored (pre-calculated) ‘join’ operation in RDBMS. They always have a type, a start and end node, and a direction.
* __Properties__ - name/value pairs that both Nodes and Relationships can contain.
* __Labels__ - are means  to quickly and efficiently create subgraphs.

### Graph DB specific use cases
* Recommender System
* Fraud Detection System
* Social Network
* Access Control  

_More to learn._
