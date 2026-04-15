# Best Bike Paths (BBP)

Requirement Engineering & System Design Project developed for the **Software Engineering 2** course.

## Overview

**Best Bike Paths (BBP)** is a software engineering project focused on the analysis and design of a platform that helps cyclists:

- record and manage personal trips
- create routes manually or through automatic sensor-based tracking
- publish routes for the community
- search and compare bike paths between an origin and a destination
- rank candidate paths based on quality, status, and effectiveness

This repository collects the complete engineering documentation produced for the project, with a strong focus on **requirements engineering, domain modeling, software architecture, traceability, and formal validation**.

## What this project shows

This project highlights the practical skills involved in:

- **requirements elicitation and specification** from an informal problem statement
- **scenario analysis and use case modeling**
- **UML-based system design**
- **architectural decomposition** using layered and microservices-oriented patterns;
- **formal modeling and verification** with Alloy
- **technical documentation in LaTeX**
- **traceability between requirements and design decisions**
- **integration and testing planning** for complex distributed systems

## Project context

The assignment required the production of two main deliverables for the **Best Bike Paths** system:

- **RASD** — Requirement Analysis and Specification Document;
- **DD** — Design Document.

## Main activities carried out

### 1. Requirements Engineering

The RASD defines the system goals, actors, assumptions, domain model, functional and non-functional requirements, interfaces, and detailed use cases.

Key work included:

- identifying the distinction between **Cyclist**, **Guest**, **Path**, and **Route**
- defining product goals and shared/world phenomena
- specifying route creation in both **manual** and **automatic** modes
- modeling community publishing and ranking logic
- describing hardware and software interfaces, including sensor usage and external weather services

### 2. UML Modeling

The documentation includes multiple UML artifacts to describe the system from different perspectives, including:

- **domain class diagrams**
- **state diagrams**
- **component diagrams**
- **deployment diagrams**
- **sequence diagrams**
- **traceability structures** between requirements and architecture

### 3. Formal Analysis

A dedicated section of the RASD presents a **formal analysis with Alloy 6**.

The model was used to:

- formalize domain constraints
- verify consistency properties of routes and paths
- reason about publication and visibility rules
- validate sample worlds and dynamic transitions of the system

This was one of the strongest parts of the project because it complements natural language and UML with a more rigorous validation layer.

### 4. Architectural Design

The DD proposes a **four-tier architecture** with a **microservices-based application layer**.

Main design choices include:

- **Presentation Tier** for the mobile user interface
- **Routing Tier** for request dispatching
- **Application Tier** organized as independent microservices
- **Data Tier** with a **database-per-service** approach

The system design also adopts:

- **RESTful APIs**;
- **API Gateway** as entry point;
- **Controller–Service–Repository** internal microservice structure;
- **HTTPS** for secure communications;
- integration with **mobile sensors** and an external **Weather API**.

### 5. UI and Integration Planning

The project also includes:

- mobile UI mockups for the most important screens
- a requirements traceability matrix
- an implementation and integration strategy
- a bottom-up testing plan for progressively validating the system

## Technologies, methods, and tools used

- **LaTeX** for document authoring and versioned technical deliverables
- **UML** for visual modeling
- **Alloy 6** for formal specification and validation
- **OpenStreetMap** as mapping reference in the system design
- **RESTful architectural style**
- **Microservices architecture**
- **Four-tier architectural model**
- **Database-per-service pattern**
- **Controller–Service–Repository pattern**
- **GitHub** for repository management and versioning
- **Overleaf** for collaborative writing and contribution tracking

## Repository structure

```text
BellomoPenninoSamarani/
├── RASD/
│   ├── Files/
│   ├── Images/
│   ├── util/
│   ├── commandsFile.tex
│   ├── main.tex
│   ├── main.bib
│   └── main.pdf
├── DD/
│   ├── Files/
│   ├── Images/
│   ├── util/
│   ├── commandsFile.tex
│   ├── main.tex
│   ├── main.bib
│   └── main.pdf
├── DeliveryFolder/
│   ├── RASDv1.pdf
│   ├── RASDv2.pdf
│   ├── DDv1.pdf
│   └── DDv2.pdf
└── README.md
```

## Folder explanation

### `RASD/`
Contains the complete material for the **Requirement Analysis and Specification Document**.

Inside this folder there are:

- the **LaTeX source files** used to write the document;
- the **compiled PDF** (`main.pdf`);
- supporting assets such as diagrams, UI mockups, and utility files.

The `Files/` subfolder contains the main textual sections of the RASD, such as:

- introduction;
- overview;
- requirements;
- Alloy analysis;
- references;
- effort spent.

### `DD/`
Contains the complete material for the **Design Document**.

Inside this folder there are:

- the **LaTeX source files** used to write the document;
- the **compiled PDF** (`main.pdf`);
- architectural diagrams, sequence diagrams, deployment views, UI figures, and utility files.

The `Files/` subfolder contains the main sections of the DD, including:

- introduction;
- architectural design;
- user interface design;
- requirements traceability;
- implementation, integration and test plan;
- references;
- effort spent.

### `DeliveryFolder/`
This folder contains the **official delivered versions of the documentation**.

It includes the versioned PDFs submitted during the course workflow:

- `RASDv1.pdf`
- `RASDv2.pdf`
- `DDv1.pdf`
- `DDv2.pdf`

This means the repository does not only preserve the final result, but also documents the **evolution of the deliverables across revisions**.

### `Images/`
Present inside both `RASD/` and `DD/`, these folders collect all visual assets used in the documentation, such as:

- UML diagrams;
- UI mockups;
- Alloy screenshots;
- deployment and architectural views.

### `util/`
Contains auxiliary LaTeX utilities and support files used to keep the documents modular and maintainable.


## Authors

- Flavio Bellomo
- Salvatore Pennino @salvosku
- Anna Samarani @annasamarani
