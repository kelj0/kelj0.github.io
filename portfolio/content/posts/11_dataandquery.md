+++
authors = ["Karlo Kegljevic"]
title = "Data Models and Query Languages"
date = "2023-09-06"
tags = ["data", "models", "database", "query"]
+++



> _The limits of my language mean the limits of my world_


Data models are perhaps the most important part of developing software, because
they have such a profound effect: not only on how the software is written, but also on
how we think about the problem that we are solving.


- SQL (Structured Query Language) Databases:
    - SQL databases are relational databases that use a structured schema to define the data model.
    - Data is organized into tables with rows and columns, and relationships between tables are established through foreign keys.
    - SQL databases are suitable for structured data with well-defined relationships.
- NoSQL (Not Only SQL) Databases:
    - NoSQL databases are designed to handle unstructured or semi-structured data, as well as scenarios where the data model is not predefined.
    - They offer more flexibility in terms of schema design, allowing you to work with data that can evolve over time.
    - NoSQL databases are categorized into several types, including document-oriented, key-value, column-family, and graph databases.
- Graph Databases:
    - Graph databases are a specialized type of NoSQL database designed to handle data with complex relationships.
    - Data is represented as nodes, edges, and properties, making them ideal for modeling and querying connected data.
    - Graph databases excel in scenarios where the relationships between data points are as important as the data itself, such as social networks, recommendation engines, and fraud detection.
    - They are optimized for traversing and querying graph structures efficiently.


All three models (document, relational, and graph) are widely used today, and each is
good in its respective domain. One model can be emulated in terms of another 
model - for example, graph data can be represented in a relational database 
but the result is often awkward. That’s why we have different systems for different 
purposes, not a single one-size-fits-all solution

Today, there are even newer ways to query data, for example GenBank which is a sequence 
database specialized to perform sequence similarity searches, which means taking one 
very long string (representing a DNA molecule) and matching it against a large database
of strings that are similar, but not identical.