# StreamVault Database Design – Conceptual & Logical Models

This repository contains a database design for **StreamVault**, a digital media library and streaming platform. The goal of this project is to demonstrate core database design concepts by translating business requirements into structured data models.

## Project Overview
StreamVault allows users to manage and stream movies, TV shows, music, podcasts, and documentaries, with features such as subscriptions, playlists, viewing history, and reviews. This project focuses on designing a robust database schema to support these functionalities.

The repository includes:
- A **UML diagram** representing the **conceptual data model**
- An **ERD diagram** representing the **logical data model**
- Supporting documentation outlining assumptions and case background

## UML Diagram – Conceptual Data Model
The UML diagram captures the **high-level structure** of the system by identifying key entities, their attributes, and relationships.  
It focuses on *what* data the system needs rather than *how* it is implemented.

Key aspects illustrated:
- Account generalization (User and Guest)
- Content generalization (Movies, Series, Albums)
- Core relationships such as subscriptions, playlists, and reviews

This diagram is useful for understanding system requirements and communicating the design with non-technical stakeholders.

## ERD – Logical Data Model
The ERD translates the conceptual design into a **database-ready structure**.  
It defines tables, primary keys, foreign keys, and junction tables needed for implementation in a relational database.

Key aspects illustrated:
- Resolution of many-to-many relationships using junction table (e.g., follows)
- Subscription lookup table
- Streaming sessions and viewing history relation
- Content classification and inheritance handling

This diagram serves as a blueprint for building the actual database schema.

## Why This Project Matters
This project demonstrates my understanding of:
- Conceptual vs. logical data modeling
- UML and ERD notation
- Generalization and Association relationships in UML
- Many-to-many relationship resolution
- Translating real-world requirements into database structures
