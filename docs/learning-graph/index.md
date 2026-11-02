---
title: Learning Graph
description: The learning graph for Transmission Lines, Fields, and Waves — 392 concepts connected by prerequisite relationships, with the reports used to build and check it
---

# Learning Graph for Transmission Lines, Fields, and Waves

This section contains the learning graph for this textbook. A learning graph is
a graph of the concepts used in the book. Each concept is a node in a network
graph, and concepts are connected by directed edges that show which concepts a
student needs to understand first.

A learning graph is the foundational data structure for intelligent textbooks
that can recommend learning paths. It works like a roadmap of concepts that
helps students reach their learning goals.

At one end of the graph are the foundational concepts, such as Complex Number,
Voltage, Cartesian Coordinates and Electric Charge, which have no
prerequisites. At the other end are the most advanced concepts in the course,
such as stub matching, waveguide attenuation and the Friis transmission
equation. To master an advanced concept you need to understand every concept it
depends on.

The graph for this book has **392 concepts** connected by **726 dependency
edges**, grouped into **14 categories**.

## Course Description

The [Course Description](../course-description.md) is the source document for
the concepts in this course. It uses the 2001 Bloom's Taxonomy to organize the
learning outcomes.

## List of Concepts

Generative AI was used to turn the course description into a
[Concept List](./concept-list.md). Each concept is a short Title Case label of
at most 32 characters.

## Concept Dependency List

The concepts and their dependencies form a Directed Acyclic Graph (DAG): no
concept depends, directly or indirectly, on itself. The DAG is available in two
formats: a [CSV file](learning-graph.csv) and a [JSON file](learning-graph.json)
in the vis-network JavaScript library format. The JSON file has `metadata`,
`groups`, `nodes` and `edges` sections, and each edge has `from` and `to`
properties, so the graph can be viewed and edited with vis-network tools.

## Analysis and Documentation

### Course Description Quality Assessment

This report rates how well the course description supports learning graph
generation. It checks the required fields, the depth of the topic list, and the
learning outcomes at each Bloom's Taxonomy level.

[View the Course Description Quality Assessment](course-description-assessment.md)

### Learning Graph Quality Validation

This report uses graph algorithms to check the structure of the learning graph:

- All 392 concepts are connected in a single graph
- The graph is a valid DAG with no cycles
- Eight foundational concepts serve as entry points
- Indegree distribution and the longest dependency chains

[View the Learning Graph Quality Validation](quality-metrics.md)

### Concept Taxonomy

To make patterns in the graph visible, each concept is assigned to one of 14
categories, and each category has its own color in the graph viewer. The
categories run from mathematical and circuit foundations, through transmission
lines and field theory, to plane waves, waveguides and antennas. Each has a
3–5 letter TaxonomyID used in the CSV file.

[View the Concept Taxonomy](concept-taxonomy.md)

### Taxonomy Distribution

This report shows how many concepts fall into each category. The goal is a
roughly balanced taxonomy in which no category holds more than 30% of the
concepts. In this book the largest category, Electrostatics, holds 12.2%.

[View the Taxonomy Distribution Report](./taxonomy-distribution.md)
