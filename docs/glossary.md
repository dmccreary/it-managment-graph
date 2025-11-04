# Glossary of Terms

This glossary provides ISO 11179-compliant definitions for all concepts in the IT Management Graph learning graph. Each definition follows ISO 11179 metadata registry guidelines: precise, concise, distinct, non-circular, and unencumbered with business rules.

#### Access Control

A security mechanism that restricts who can view or modify specific data or system resources based on defined permissions.

**See also:** Role-Based Access Control, Security Model

#### Accuracy

A data quality dimension measuring the degree to which data correctly represents the real-world entities or events it describes.

**Example:** An asset database showing server PROD-01 has 64GB RAM when it actually has 128GB fails the accuracy criterion.

#### AI-Assisted Curation

The application of machine learning algorithms to automate the review, classification, and quality improvement of data within management systems.

**Example:** An AI system automatically flags CMDB entries with missing dependency relationships for human review.

#### Anomaly Detection

The use of algorithms, often machine learning-based, to identify data patterns that deviate significantly from expected norms.

**See also:** Data Validation, Machine Learning

#### Application Dependency

A relationship where one software application relies on another application to function properly.

**Example:** The checkout application depends on the payment processing application to complete customer transactions.

#### Application Portfolio

The complete collection of software applications owned and operated by an organization.

**See also:** Digital Estate, IT Portfolio

#### Artificial Intelligence

The capability of computer systems to perform tasks that typically require human intelligence, such as learning, reasoning, and pattern recognition.

**See also:** Machine Learning, Graph RAG

#### Asset Management

The systematic approach to tracking, maintaining, and optimizing the value and lifecycle of organizational assets.

**Example:** Asset management tracks all servers from procurement through deployment to decommissioning.

#### Atlassian

A software company providing collaboration and project management tools including Jira, Confluence, and IT service management solutions.

#### Audit Trail

A chronological record of system activities and changes that enables reconstruction of events for security or compliance purposes.

**Example:** The CMDB audit trail shows who changed the server configuration and when, supporting compliance investigations.

**See also:** Compliance Reporting

#### Auto-Discovery

Abbreviated term for Automated Discovery.

**See also:** Automated Discovery

#### Automated Discovery

The capability of systems to automatically detect and catalog IT resources, configurations, and relationships without manual intervention.

**Example:** Discovery tools scan the network every hour to automatically update the topology map with new devices.

**See also:** OpenTelemetry, eBPF

#### Best Practice

A technique or methodology that through experience and research has proven to reliably lead to desired outcomes.

**See also:** Industry Standard, Framework Adoption

#### Blast Radius

The set of all IT resources and business services potentially affected when a specific component fails or changes.

**Example:** When database DB-PROD-01 fails, its blast radius includes 15 microservices and 3 business capabilities.

**See also:** Impact Analysis, Downstream Dependency

#### Breadth-First Search

A graph traversal algorithm that explores all nodes at the current depth level before moving to nodes at the next depth level.

**See also:** Depth-First Search, Graph Traversal

#### Build vs Buy

The strategic decision framework for determining whether to develop a capability in-house or purchase an existing solution.

**See also:** Vendor Evaluation, Technology Selection

#### Business Case

A structured justification for a proposed initiative that evaluates costs, benefits, risks, and alternative approaches.

**See also:** Return on Investment, Total Cost of Ownership

#### Business Rule

A statement that defines or constrains some aspect of business operations, describing what must or must not occur.

**Example:** A business rule might state that all production servers must have automated backups configured.

#### Business Service

An IT-supported capability that delivers value to business stakeholders and supports business processes.

**Example:** The "Customer Order Processing" business service depends on multiple technical services including databases and payment systems.

**See also:** Technical Service, Service Mapping

#### Business Service Mapping

The process of identifying and documenting relationships between business services and their underlying technical components.

**Example:** Mapping shows that the "Online Banking" business service depends on 12 technical services and 47 infrastructure components.

**See also:** Service Mapping, Service Topology

#### Capability Model

A structured representation of an organization's abilities to perform specific functions or processes at varying levels of maturity.

**See also:** Process Maturity

#### Change Impact Assessment

The analysis of potential effects that a proposed change may have on interconnected systems and business services.

**Example:** Before upgrading the database, impact assessment reveals 23 dependent applications requiring testing.

**See also:** Impact Analysis, Change Management

#### Change Management

The systematic approach to controlling and coordinating modifications to IT infrastructure in a standardized and traceable manner.

**Example:** All production changes must follow the change management process including approval, testing, and rollback planning.

**See also:** ITIL, Service Support

#### Circular Dependency

A situation where two or more components depend on each other either directly or through a chain of dependencies, forming a cycle.

**Example:** Service A depends on Service B, which depends on Service C, which depends back on Service A.

**See also:** Directed Acyclic Graph, Dependency Chain

#### Classification System

A scheme for organizing items into categories based on shared characteristics or properties.

**See also:** Taxonomy

#### CMDB

Acronym for Configuration Management Database.

**See also:** Configuration Management Database, Configuration Management

#### Column

A vertical element in a relational database table representing a specific attribute or data field that stores values of the same type.

**See also:** Table, Row, Database Schema

#### Completeness

A data quality dimension measuring the degree to which all required data values are present and populated.

**Example:** A CMDB entry missing the server's operating system version fails the completeness criterion.

**See also:** Accuracy, Data Quality Dimension

#### Compliance

Adherence to laws, regulations, industry standards, and organizational policies governing operations and data management.

**See also:** Regulatory Compliance, HIPAA, GDPR, DORA

#### Compliance Reporting

The systematic generation of documentation demonstrating adherence to regulatory requirements and organizational policies.

**Example:** Quarterly compliance reports show all servers meet HIPAA encryption requirements by querying the CMDB.

**See also:** Audit Trail, Regulatory Compliance

#### Configuration Audit

A formal review process that verifies actual configuration states match documented baselines and approved specifications.

**See also:** Configuration Baseline, Configuration Management

#### Configuration Baseline

An approved and documented specification of configuration attributes at a specific point in time, used as a reference for comparison.

**Example:** The production baseline documents that all web servers should run Ubuntu 22.04 with specific security patches.

**See also:** Configuration Audit

#### Configuration Drift

The divergence of actual system configurations from their documented or intended state over time.

**Example:** Servers configured identically at deployment now show different package versions, indicating configuration drift.

**See also:** Drift Detection, Configuration Baseline

#### Configuration Item

An IT resource, asset, or component that is identified, tracked, and managed within a configuration management system.

**Example:** A physical server, virtual machine, software license, or network switch can each be a configuration item.

**See also:** Configuration Management, Asset Management

#### Configuration Management

The discipline of identifying, organizing, controlling, and documenting IT resources and their relationships throughout the lifecycle.

**Example:** Configuration management tracks what servers exist, their specifications, and how they connect to applications.

**See also:** Configuration Item, CMDB, ITIL

#### Configuration Management Database

A repository that stores information about configuration items, their attributes, and relationships in an IT environment.

**Example:** The CMDB stores data about 5,000 servers, their installed software, and connections to 200 applications.

**See also:** CMDB, Configuration Management

#### Consistency

A data quality dimension measuring the degree to which data values agree across different systems and over time.

**Example:** The same server ID returning different hostnames in different databases indicates a consistency issue.

**See also:** Data Quality Dimension

#### Continuous Improvement

An ongoing effort to incrementally enhance processes, products, or services through systematic analysis and refinement.

**See also:** Operational Excellence, Best Practice

#### Cycle Detection

An algorithm that identifies circular dependencies or loops within a directed graph structure.

**Example:** Cycle detection reveals that three microservices have circular dependencies that should be refactored.

**See also:** Circular Dependency, Directed Acyclic Graph

#### Cypher Query Language

A declarative query language designed specifically for querying and manipulating graph databases, particularly Neo4j.

**Example:** The Cypher query `MATCH (s:Server)-[:DEPENDS_ON*]->(d) RETURN d` finds all transitive dependencies of a server.

**See also:** Neo4j, Graph Query

#### DAG

Acronym for Directed Acyclic Graph.

**See also:** Directed Acyclic Graph

#### Data Catalog

A centralized inventory of data assets with metadata describing their content, location, ownership, and usage.

**See also:** Metadata, Data Governance

#### Data Custodian

An individual or team responsible for the technical management and security of data systems and storage.

**See also:** Data Owner, Data Steward

#### Data Governance

The framework of policies, procedures, roles, and standards for managing data quality, security, and usage as an organizational asset.

**Example:** Data governance establishes who can approve changes to the CMDB and what validation rules apply.

**See also:** Data Management, Data Quality, Data Steward

#### Data Lineage

The documentation of data's origins, transformations, and movement through systems from creation to consumption.

**Example:** Data lineage traces how server configuration data flows from discovery tools through the CMDB to reporting dashboards.

**See also:** Metadata, Data Governance

#### Data Management

The discipline of collecting, storing, organizing, maintaining, and using data effectively and securely across the organization.

**See also:** Data Governance, DMBOK

#### Data Migration

The process of moving data from one system, format, or location to another, typically during system upgrades or consolidation.

**Example:** Migrating from a legacy CMDB to a graph-based system requires transforming relational tables into nodes and edges.

**See also:** Legacy Migration, System Cutover

#### Data Owner

An individual or role with authority and accountability for data quality, access decisions, and usage policies for specific data domains.

**See also:** Data Steward, Data Governance

#### Data Quality

The fitness of data for its intended purposes, measured across dimensions including accuracy, completeness, and timeliness.

**Example:** A CMDB with 40% accuracy cannot support reliable impact analysis for incident response.

**See also:** Data Quality Dimension, Fitness for Purpose

#### Data Quality Dimension

A specific aspect of data quality used for measurement, such as accuracy, completeness, consistency, timeliness, or validity.

**See also:** Accuracy, Completeness, Consistency, Timeliness, Validity

#### Data Steward

An individual responsible for ensuring data quality, defining standards, and facilitating proper data usage within a domain.

**See also:** Data Owner, Data Governance

#### Data Validation

The process of checking data against defined rules, constraints, and formats to ensure correctness and quality.

**Example:** Data validation rejects CMDB entries where the server IP address format is invalid.

**See also:** Validation Rule, Data Quality

#### Database Index

A data structure that improves the speed of data retrieval operations on database tables at the cost of additional storage and slower writes.

**See also:** Query Performance, Query Optimization

#### Database Schema

The formal description of how data is organized in a database, including tables, columns, data types, and relationships.

**Example:** The CMDB schema defines tables for servers, applications, and relationships between them.

**See also:** Table, Column, Schema Rigidity

#### Dependency Chain

A sequence of components where each depends on the next, forming a path through the dependency graph.

**Example:** The web application depends on the API service, which depends on the database, forming a three-element chain.

**See also:** Dependency Map, Transitive Dependency

#### Dependency Map

A visual representation showing how IT components depend on one another across the infrastructure.

**Example:** The dependency map reveals that 15 applications ultimately depend on a single aging database server.

**See also:** Dependency Chain, Service Topology

#### Dependency Tracing

The process of following relationships in a graph to identify all components connected through dependency relationships.

**Example:** Dependency tracing from a failed database identifies all affected applications within seconds using graph queries.

**See also:** Upstream Dependency, Downstream Dependency, Graph Traversal

#### Depth-First Search

A graph traversal algorithm that explores as far as possible along each branch before backtracking to explore other branches.

**See also:** Breadth-First Search, Graph Traversal

#### Digital Estate

The comprehensive inventory of all digital and IT assets owned or managed by an organization.

**See also:** Application Portfolio, IT Portfolio

#### Digital Operational Resilience Act

An EU regulation requiring financial entities to ensure information and communication technology security and operational resilience.

**See also:** DORA, Regulatory Compliance

#### Digital Transformation

The strategic integration of digital technology into all areas of business operations to fundamentally change how value is delivered.

**Example:** Digital transformation replaces manual CMDB updates with automated discovery and AI-assisted data quality management.

**See also:** IT Modernization, Business Case

#### Directed Acyclic Graph

A directed graph containing no cycles, meaning there is no path that starts and ends at the same node.

**Example:** A proper IT dependency graph should be a DAG to avoid circular dependencies that prevent clean service startup.

**See also:** DAG, Directed Graph, Cycle Detection

#### Directed Graph

A graph structure where each edge has a specific direction, pointing from one node to another.

**Example:** In an IT dependency graph, edges point from dependent services to the services they depend on.

**See also:** Undirected Graph, Edge, Node

#### DMBOK

Acronym for Data Management Body of Knowledge, a comprehensive framework for data management practices.

**See also:** Data Management, Data Governance

#### DORA

Acronym for Digital Operational Resilience Act.

**See also:** Digital Operational Resilience Act

#### Downstream Dependency

A component or service that depends on the current component, potentially affected if the current component fails or changes.

**Example:** The downstream dependencies of the payment database include all checkout and order processing services.

**See also:** Upstream Dependency, Blast Radius

#### Drift Detection

The automated identification of configuration changes that cause systems to deviate from their intended or baseline state.

**Example:** Drift detection alerts when production servers no longer match their documented configuration baseline.

**See also:** Configuration Drift, Automated Discovery

#### Dynamic Topology

The real-time representation of IT infrastructure and service relationships that automatically updates as components and connections change.

**Example:** Dynamic topology mapping continuously updates as containers are created and destroyed in a Kubernetes cluster.

**See also:** Network Topology, Service Topology, Automated Discovery

#### Dynatrace

A software intelligence platform providing application performance monitoring, infrastructure monitoring, and full-stack observability capabilities.

**See also:** Monitoring, Observability

#### eBPF

Acronym for extended Berkeley Packet Filter.

**See also:** Extended Berkeley Packet Filter

#### Edge

A connection or link between two nodes in a graph representing a relationship, association, or dependency.

**Example:** In an IT dependency graph, an edge from App A to Database B represents "App A depends on Database B."

**See also:** Node, Relationship, Directed Graph

#### Edge Property

An attribute or metadata value associated with an edge in a property graph.

**Example:** An edge property might store "criticality: high" on the dependency relationship between a revenue system and its database.

**See also:** Property Graph, Node Property

#### Exception Reporting

The systematic identification and notification of data or conditions that violate defined rules or fall outside expected parameters.

**Example:** Exception reports flag all CMDB entries missing required fields or containing invalid relationship types.

**See also:** Data Quality, Validation Rule

#### Extended Berkeley Packet Filter

A technology enabling custom programs to run safely in operating system kernels for high-performance monitoring, networking, and security.

**Example:** eBPF programs capture every network connection in real-time to auto-discover service dependencies without agents.

**See also:** eBPF, Telemetry, Automated Discovery

#### Fitness for Purpose

A data quality measure assessing whether data is suitable and adequate for its intended use case.

**Example:** CMDB data accurate enough for asset tracking may not have sufficient detail for automated incident resolution.

**See also:** Data Quality

#### Foreign Key

A column or set of columns in one database table that uniquely identifies rows in another table, establishing a relationship between tables.

**Example:** The "server_id" column in the applications table is a foreign key referencing the "id" column in the servers table.

**See also:** Primary Key, Table, Join Operation

#### Framework Adoption

The process of implementing and integrating established methodologies or best practice frameworks into organizational operations.

**Example:** Framework adoption involves training staff on ITIL processes and customizing them to organizational needs.

**See also:** ITIL, Best Practice

#### GDPR

Acronym for General Data Protection Regulation.

**See also:** General Data Protection Regulation

#### General Data Protection Regulation

A comprehensive European Union regulation establishing requirements for the collection, processing, and protection of personal data.

**See also:** GDPR, Regulatory Compliance, Compliance

#### Graph Algorithm

A computational procedure designed to solve problems or perform analyses on graph structures.

**Example:** Graph algorithms can find the shortest path between nodes or identify all components within N hops of a starting point.

**See also:** Graph Traversal, Path Finding

#### Graph Complexity

A measure of how intricate or computationally challenging a graph structure is based on factors like size, density, and connectivity patterns.

**See also:** Graph Density, Node Degree

#### Graph Database

A database that uses graph structures with nodes, edges, and properties to represent and store data, optimized for relationship queries.

**Example:** A graph database stores servers as nodes and dependencies as edges, enabling instant multi-hop dependency queries.

**See also:** Property Graph, Neo4j, Native Graph Storage

#### Graph Density

The ratio of actual edges to possible edges in a graph, indicating how interconnected the nodes are.

**Example:** A highly dense IT dependency graph suggests tight coupling that may complicate changes and increase blast radius.

**See also:** Graph Complexity, Edge

#### Graph Layer

A graph-oriented interface or processing layer built on top of a non-graph storage system like a relational database.

**Example:** Some vendors provide a graph query layer over their existing RDBMS-based CMDB rather than native graph storage.

**See also:** Native Graph Storage, Graph Database

#### Graph Metric

A quantitative measure characterizing properties of a graph structure such as density, centrality, or clustering coefficient.

**See also:** Graph Complexity, Node Degree

#### Graph Query

A database operation that leverages graph structure to find patterns, paths, or relationships between nodes.

**Example:** A graph query finds all servers within three dependency hops of a specific application in milliseconds.

**See also:** Cypher Query Language, Pattern Matching, Graph Traversal

#### Graph RAG

A retrieval-augmented generation approach that combines graph databases with large language models to provide context-aware AI responses.

**Example:** Graph RAG uses the IT dependency graph to provide accurate answers about which services would be affected by planned maintenance.

**See also:** Retrieval Augmented Generation, Knowledge Graph

#### Graph Theory

The mathematical study of graphs as abstract structures consisting of vertices connected by edges.

**Example:** Graph theory provides the algorithms and principles underlying efficient dependency analysis in IT management systems.

**See also:** Node, Edge, Graph Database

#### Graph Traversal

The process of systematically visiting nodes in a graph by following edges according to a specific strategy or pattern.

**Example:** Graph traversal from a database node visits all dependent applications by following dependency edges.

**See also:** Depth-First Search, Breadth-First Search, Path Finding

#### Hardware Asset

A physical IT resource such as a server, network device, storage system, or end-user device.

**Example:** A Dell PowerEdge server is a hardware asset tracked in the asset management system.

**See also:** IT Asset, Software Asset

#### Health Insurance Portability

The full name of HIPAA, referring to the act's provisions for healthcare coverage continuity and data privacy.

**See also:** HIPAA

#### HIPAA

Acronym for Health Insurance Portability and Accountability Act, a US law establishing privacy and security standards for health information.

**Example:** HIPAA compliance requires tracking which systems store patient data and ensuring appropriate access controls.

**See also:** Health Insurance Portability, Regulatory Compliance

#### Horizontal Scaling

Increasing system capacity by adding more machines or instances rather than upgrading existing hardware.

**Example:** Horizontal scaling adds five more web servers to handle increased load rather than upgrading to larger servers.

**See also:** Vertical Scaling, Scalability

#### Impact Analysis

The systematic assessment of potential effects from a change, failure, or incident by tracing through dependency relationships.

**Example:** Impact analysis before database maintenance reveals 12 applications requiring notification and service windows.

**See also:** Blast Radius, Change Impact Assessment, Root Cause Analysis

#### In-Degree

The number of edges pointing into a node in a directed graph, indicating how many other nodes depend on it.

**Example:** A database with high in-degree indicates many applications depend on it, making it critical infrastructure.

**See also:** Out-Degree, Node Degree, Directed Graph

#### Incident Management

The process of restoring normal service operation as quickly as possible following an unplanned interruption or service degradation.

**Example:** Incident management uses the dependency graph to quickly identify the root cause and affected services.

**See also:** ITIL, Problem Management, Incident Response

#### Incident Response

The systematic approach to handling security breaches, system failures, or service interruptions to minimize damage and restore operations.

**Example:** Incident response teams query the graph database to instantly identify the blast radius of a database failure.

**See also:** Incident Management, Mean Time to Detect

#### Industry Standard

A widely accepted specification, protocol, or practice established through formal consensus or common adoption across an industry.

**See also:** Best Practice, Framework Adoption

#### Information Technology Infrastructure Library

A comprehensive framework of best practices for IT service management originally developed by the UK government.

**Example:** ITIL provides process frameworks for configuration management, incident management, and change management.

**See also:** ITIL, Service Support, Service Delivery

#### Infrastructure Dependency

A relationship where a service or application relies on underlying infrastructure components such as networks, servers, or storage.

**Example:** The web application has infrastructure dependencies on load balancers, web servers, and network connectivity.

**See also:** Application Dependency, Technical Service

#### Inner Join

A relational database operation that returns only rows where matching values exist in both tables being joined.

**Example:** An inner join between servers and applications tables returns only servers that have applications installed.

**See also:** Outer Join, Join Operation

#### IT Asset

Any technology resource owned or managed by an organization including hardware, software, and digital resources.

**Example:** Servers, software licenses, and network equipment are all IT assets tracked in the asset management system.

**See also:** Hardware Asset, Software Asset, Configuration Item

#### IT Modernization

The process of updating legacy systems, processes, and technologies to contemporary platforms and approaches.

**Example:** IT modernization replaces the relational CMDB with a graph database for real-time dependency analysis.

**See also:** Digital Transformation, Legacy Migration

#### IT Portfolio

The complete collection of IT assets, applications, services, and investments managed by an organization.

**See also:** Application Portfolio, Digital Estate

#### ITIL

Acronym for Information Technology Infrastructure Library.

**See also:** Information Technology Infrastructure Library

#### ITIL Version 1

The original 1989-1990 release of ITIL focusing on IT service management best practices developed for UK government agencies.

**See also:** ITIL, Service Support, Service Delivery

#### Join Operation

A relational database operation that combines rows from two or more tables based on related columns.

**Example:** Joining the servers table with the applications table shows which applications run on each server.

**See also:** Inner Join, Outer Join, Foreign Key

#### Key Performance Indicator

A measurable value that demonstrates how effectively an organization or function achieves key business objectives.

**Example:** Mean time to resolve incidents is a KPI measuring IT operations effectiveness.

**See also:** KPI, Performance Metric

#### Knowledge Graph

A graph structure that represents entities, concepts, and their semantic relationships to enable advanced reasoning and query capabilities.

**Example:** A knowledge graph of IT infrastructure connects technical components to business capabilities and compliance requirements.

**See also:** Property Graph, Ontology, Graph RAG

#### KPI

Acronym for Key Performance Indicator.

**See also:** Key Performance Indicator

#### Legacy Migration

The process of transitioning from outdated systems and platforms to modern technologies.

**Example:** Legacy migration from a relational CMDB to a graph database requires data transformation and process changes.

**See also:** IT Modernization, Migration Strategy, Data Migration

#### Legacy System

An outdated computing system, application, or technology that remains in use despite newer alternatives being available.

**Example:** The 15-year-old CMDB built on Oracle is a legacy system requiring significant manual maintenance.

**See also:** Technical Debt, IT Modernization

#### Machine Learning

A subset of artificial intelligence where systems improve performance on tasks through experience and data without explicit programming.

**Example:** Machine learning models predict which CMDB relationships are likely incorrect based on historical correction patterns.

**See also:** Artificial Intelligence, AI-Assisted Curation

#### Master Data Management

The discipline of creating and maintaining consistent, accurate, and authoritative master data across the enterprise.

**Example:** Master data management ensures the same server has one canonical record across all IT systems.

**See also:** Data Management, Reference Data

#### Mean Time to Detect

The average duration between when an incident occurs and when it is first identified or detected by monitoring systems or personnel.

**Example:** Improved observability reduced mean time to detect from 45 minutes to 3 minutes for critical service failures.

**See also:** MTTD, Mean Time to Resolve, Incident Response

#### Mean Time to Resolve

The average duration from incident detection to full restoration of normal service operation.

**Example:** Graph-based dependency tracing reduced mean time to resolve by enabling faster root cause identification.

**See also:** MTTR, Mean Time to Detect, Incident Management

#### Metadata

Structured information that describes, explains, locates, or otherwise characterizes other data resources.

**Example:** Metadata for a CMDB table includes column names, data types, update timestamps, and data owner information.

**See also:** Data Lineage, Data Catalog

#### Migration Strategy

A planned approach for transitioning from current systems or architectures to target future states.

**Example:** The migration strategy phases the transition from relational CMDB to graph database over 18 months.

**See also:** Legacy Migration, Data Migration

#### Military-Spec Configuration

Configuration management practices derived from military and defense industry standards emphasizing strict version control and documentation.

**Example:** Military-spec configuration management tracks every hardware component revision, which is excessive for dynamic cloud infrastructure.

**See also:** Configuration Management

#### Monitoring

The continuous observation and collection of metrics, logs, and events to track the health, performance, and behavior of systems.

**Example:** Monitoring collects CPU, memory, and network metrics from all servers every 30 seconds.

**See also:** Observability, Telemetry

#### MTTD

Acronym for Mean Time to Detect.

**See also:** Mean Time to Detect

#### MTTR

Acronym for Mean Time to Resolve.

**See also:** Mean Time to Resolve

#### Multi-Hop Query

A database query that traverses multiple relationship levels to find indirectly connected data.

**Example:** A multi-hop query finds all infrastructure components three or more levels removed from a business service.

**See also:** Transitive Dependency, Graph Traversal

#### Native Graph Storage

A database storage architecture specifically designed for graph structures, storing nodes and edges directly rather than mapping them to tables.

**Example:** Neo4j uses native graph storage, enabling faster traversals than graph layers built on relational databases.

**See also:** Graph Database, Graph Layer

#### Neo4j

A leading native graph database platform that uses the Cypher query language and is widely adopted for knowledge graphs and network analysis.

**Example:** Neo4j stores the IT dependency graph with servers as nodes and dependencies as relationships.

**See also:** Graph Database, Cypher Query Language, Native Graph Storage

#### Network Topology

The arrangement and interconnection of network devices and communication paths in an infrastructure.

**Example:** Network topology mapping shows how routers, switches, and firewalls connect to form the corporate network.

**See also:** Service Topology, Infrastructure Dependency

#### Node

A fundamental unit in a graph structure representing an entity, object, or data point.

**Example:** In an IT dependency graph, each server, application, and database is represented as a node.

**See also:** Edge, Vertex, Graph Database

#### Node Degree

The number of edges connected to a node in a graph.

**Example:** A database node with high degree has many connections, indicating it's heavily used or central to the architecture.

**See also:** In-Degree, Out-Degree

#### Node Property

An attribute or data field associated with a node in a property graph.

**Example:** Node properties for a server include hostname, IP address, operating system, and CPU count.

**See also:** Property Graph, Edge Property

#### Observability

The ability to measure and understand the internal state and behavior of a system based on its external outputs including metrics, logs, and traces.

**Example:** Observability enables understanding why application latency increased by examining traces through the entire dependency chain.

**See also:** Monitoring, Telemetry, OpenTelemetry

#### Ontology

A formal representation of knowledge defining entities, attributes, and relationships within a domain using a shared vocabulary.

**Example:** An IT ontology defines that "Server" is a type of "Hardware Asset" and can have relationships like "hosts" to "Application."

**See also:** Taxonomy, Knowledge Graph, Semantic Model

#### OpenTelemetry

An open-source observability framework providing standardized instrumentation, collection, and export of telemetry data including metrics, logs, and traces.

**Example:** OpenTelemetry agents automatically capture service-to-service communications to build an accurate dependency graph.

**See also:** Telemetry, Observability, Automated Discovery

#### Operational Excellence

The systematic pursuit of superior performance through process improvement, measurement, and adherence to best practices.

**See also:** Continuous Improvement, Best Practice

#### Out-Degree

The number of edges pointing out from a node in a directed graph, indicating how many other nodes it depends on.

**Example:** An application with high out-degree depends on many other services, making it potentially fragile.

**See also:** In-Degree, Node Degree, Directed Graph

#### Outer Join

A relational database operation that returns all rows from one table and matching rows from another, with nulls where no match exists.

**Example:** An outer join between servers and applications shows all servers including those without any applications installed.

**See also:** Inner Join, Join Operation

#### Path Finding

The process of identifying a route or sequence of edges connecting two nodes in a graph.

**Example:** Path finding algorithms discover the dependency chain from a business service down to specific infrastructure components.

**See also:** Shortest Path, Graph Traversal

#### Pattern Matching

The technique of searching for specific structural configurations or sequences within data, particularly in graph queries.

**Example:** Pattern matching in Cypher finds all instances where an application depends on a database that depends on shared storage.

**See also:** Graph Query, Cypher Query Language

#### Performance Metric

A quantitative measure used to assess the efficiency, speed, or resource utilization of a system or process.

**See also:** Query Performance, Key Performance Indicator

#### Policy Enforcement

The automated or manual application of rules and controls to ensure compliance with organizational policies.

**Example:** Policy enforcement automatically blocks CMDB changes that would violate data governance rules.

**See also:** Data Governance, Business Rule

#### Primary Key

A unique identifier for each record in a database table that cannot contain null values or duplicates.

**Example:** The "server_id" column serves as the primary key uniquely identifying each server in the table.

**See also:** Foreign Key, Table

#### Problem Management

The process of identifying and addressing the root causes of incidents to prevent recurrence and minimize impact.

**Example:** Problem management analyzes recurring database incidents and discovers inadequate capacity planning as the root cause.

**See also:** Incident Management, Root Cause Analysis

#### Process Maturity

The degree to which organizational processes are explicitly defined, managed, measured, and continuously improved.

**See also:** Capability Model, Continuous Improvement

#### Property Graph

A graph model where both nodes and edges can have associated properties or attributes storing additional information.

**Example:** In a property graph, a server node has properties like "hostname" and "CPU_count" while dependency edges have "criticality" properties.

**See also:** Node Property, Edge Property, Graph Database

#### Query Latency

The time delay between submitting a database query and receiving the complete result set.

**Example:** Query latency for multi-hop dependency queries is 50ms in graph databases versus 5 seconds in relational databases.

**See also:** Response Time, Real-Time Query

#### Query Optimization

The process of improving database query performance through techniques like index usage, query rewriting, and execution plan tuning.

**See also:** Query Performance, Database Index

#### Query Performance

The speed and efficiency with which a database system executes queries and returns results.

**Example:** Graph databases provide superior query performance for multi-hop dependency traversals compared to relational joins.

**See also:** Query Latency, Performance Metric

#### RBAC

Acronym for Role-Based Access Control.

**See also:** Role-Based Access Control

#### RDBMS

Acronym for Relational Database Management System, a software system that manages data using the relational model.

**Example:** Oracle, PostgreSQL, and MySQL are popular RDBMS platforms that organize data into tables with rows and columns.

**See also:** Relational Database, SQL, Database Schema

#### Real-Time Query

A database query that executes and returns results quickly enough to support immediate decision-making, typically within seconds or sub-second.

**Example:** Real-time queries enable incident responders to instantly see the blast radius of a failing component.

**See also:** Query Latency, Response Time

#### Reference Data

Standardized, relatively static data used for classification and categorization across systems, such as country codes or product types.

**See also:** Master Data Management

#### Regulatory Compliance

Adherence to laws, regulations, and mandates issued by government or regulatory bodies governing specific industries or activities.

**Example:** Financial services firms must demonstrate regulatory compliance with DORA by maintaining accurate IT asset inventories.

**See also:** Compliance, HIPAA, GDPR, DORA

#### Relational Database

A database system that organizes data into tables with rows and columns, where relationships between data are established through key constraints and join operations.

**Example:** Traditional CMDBs built on relational databases struggle with multi-hop dependency queries that require multiple expensive join operations.

**See also:** RDBMS, Table, SQL, Graph Database

#### Relationship

A named connection or association between two entities in a data model or graph structure.

**Example:** The "DEPENDS_ON" relationship connects an application node to the database node it requires.

**See also:** Edge, Property Graph

#### Release Management

The process of planning, scheduling, and controlling the deployment of software releases and updates across environments.

**See also:** Change Management, Service Delivery

#### Response Time

The total elapsed time from when a request is made until a complete response is received.

**See also:** Query Latency, Performance Metric

#### Retrieval Augmented Generation

An AI technique that enhances language model outputs by retrieving relevant information from external knowledge sources before generating responses.

**Example:** Retrieval augmented generation queries the IT dependency graph to provide accurate answers about infrastructure relationships.

**See also:** Graph RAG, Knowledge Graph

#### Return on Investment

A financial metric calculating the ratio of net profit to initial investment cost, expressed as a percentage or ratio.

**Example:** The graph database migration showed 300% ROI through reduced incident resolution time and eliminated CMDB maintenance costs.

**See also:** ROI, Total Cost of Ownership, Business Case

#### Risk Assessment

The systematic process of identifying, analyzing, and evaluating potential risks to determine their likelihood and potential impact.

**See also:** Risk Management, Vendor Management

#### Risk Management

The coordinated activities to identify, assess, mitigate, and monitor risks to organizational objectives.

**See also:** Risk Assessment, Compliance

#### ROI

Acronym for Return on Investment.

**See also:** Return on Investment

#### Role-Based Access Control

A security model that grants system access and permissions based on a user's assigned roles rather than individual identity.

**Example:** Users with the "Database Administrator" role can modify database configuration items while developers have read-only access.

**See also:** RBAC, Access Control

#### Root Cause Analysis

The systematic investigation to identify the fundamental reason why an incident or problem occurred, not just its symptoms.

**Example:** Root cause analysis using dependency tracing revealed that database failures stemmed from inadequate storage capacity.

**See also:** Problem Management, Dependency Tracing

#### Row

A horizontal record in a relational database table representing a single instance or entity with values for each column.

**See also:** Table, Column

#### Scalability

The capability of a system to handle increased load or demand by adding resources without significant performance degradation.

**See also:** Horizontal Scaling, Vertical Scaling

#### Schema Evolution

The process of modifying database schema structure over time to accommodate changing requirements while maintaining data integrity.

**Example:** Schema evolution in relational databases requires careful migration planning, while graph databases more easily adapt to new relationship types.

**See also:** Schema Rigidity, Database Schema

#### Schema Rigidity

The characteristic of database schemas, particularly relational, that require significant effort and planning to modify their structure.

**Example:** Schema rigidity in the CMDB makes it difficult to quickly add new asset types or relationship categories.

**See also:** Schema Evolution, Database Schema

#### Security Model

A framework defining how access control, authentication, and authorization are implemented and enforced within a system.

**See also:** Role-Based Access Control, Access Control

#### Semantic Model

A representation of data that captures meaning and relationships using formal semantics enabling reasoning and inference.

**See also:** Ontology, Knowledge Graph

#### Service Delivery

One of two core focus areas in ITIL Version 1, encompassing processes for planning and delivering IT services to meet business needs.

**See also:** Service Support, ITIL

#### Service Dependency

A relationship where one IT service relies on another service to function correctly.

**Example:** The email service has service dependencies on the authentication service and storage service.

**See also:** Application Dependency, Infrastructure Dependency

#### Service Level Agreement

A formal commitment between a service provider and customer specifying expected service quality, availability, and responsibilities.

**Example:** The SLA guarantees 99.9% availability for the customer portal service with 15-minute response time for critical incidents.

**See also:** SLA

#### Service Mapping

The practice of identifying and documenting relationships between IT services and their underlying technical components.

**Example:** Service mapping reveals that the order processing service depends on 8 applications, 15 servers, and 2 databases.

**See also:** Business Service Mapping, Dependency Map

#### Service Support

One of two core focus areas in ITIL Version 1, encompassing operational processes including incident, problem, and change management.

**See also:** Service Delivery, ITIL, Incident Management

#### Service Topology

The arrangement and relationships of IT services showing how they connect and depend on one another.

**Example:** Service topology visualization shows how 50 microservices interconnect to deliver customer-facing capabilities.

**See also:** Network Topology, Service Mapping

#### ServiceNow

A leading enterprise platform providing IT service management, workflow automation, and configuration management database capabilities.

**Example:** Many organizations use ServiceNow's CMDB as their central repository for IT asset and configuration data.

**See also:** CMDB, Vendor Management

#### Shortest Path

The minimum-length route between two nodes in a graph as measured by number of edges or weighted edge costs.

**Example:** Finding the shortest path from a business service to failed infrastructure helps quickly identify the dependency chain.

**See also:** Path Finding, Graph Algorithm

#### SLA

Acronym for Service Level Agreement.

**See also:** Service Level Agreement

#### Software Asset

A licensed or developed software program, application, or code component owned or used by an organization.

**Example:** Microsoft Office licenses and custom Java applications are both software assets tracked in the asset inventory.

**See also:** IT Asset, Hardware Asset

#### SQL

Acronym for Structured Query Language.

**See also:** Structured Query Language

#### Structured Query Language

A standardized declarative programming language for creating, querying, and managing data in relational database systems.

**Example:** SQL queries require complex JOIN operations to trace multi-hop dependencies in relational CMDBs.

**See also:** SQL, RDBMS

#### System Cutover

The transition point when operations switch from an old system to a new replacement system.

**Example:** The system cutover from legacy CMDB to graph database occurred during a planned maintenance window.

**See also:** Migration Strategy, Data Migration

#### System Integration

The process of connecting different IT systems and applications to function as a coordinated whole.

**See also:** Application Dependency, Technical Service

#### Table

A collection of related data organized in rows and columns within a relational database.

**Example:** The "servers" table stores one row per server with columns for hostname, IP address, and operating system.

**See also:** Row, Column, Database Schema

#### Taxonomy

A hierarchical classification scheme organizing concepts or entities into categories based on shared characteristics.

**Example:** The IT asset taxonomy classifies resources as hardware, software, or services with multiple subcategories under each.

**See also:** Classification System, Ontology

#### TCO

Acronym for Total Cost of Ownership.

**See also:** Total Cost of Ownership

#### Technical Debt

The implied cost of future rework caused by choosing expedient solutions now instead of better approaches that would take longer.

**Example:** Building a custom CMDB on an aging RDBMS creates technical debt that eventually requires expensive migration.

**See also:** Legacy System, IT Modernization

#### Technical Service

An IT service that provides infrastructure capabilities supporting business services, typically not directly visible to end users.

**Example:** Database services and authentication services are technical services supporting customer-facing business services.

**See also:** Business Service, Infrastructure Dependency

#### Technology Selection

The process of evaluating and choosing specific technologies, platforms, or tools to meet organizational requirements.

**See also:** Build vs Buy, Vendor Evaluation

#### Telemetry

Automated measurement and transmission of data from remote sources to monitoring systems for analysis.

**Example:** Telemetry from application instrumentation automatically discovers service dependencies by observing actual network communications.

**See also:** OpenTelemetry, Monitoring, Observability

#### Timeliness

A data quality dimension measuring whether data is available when needed and reflects the current state appropriately.

**Example:** A CMDB updated monthly fails the timeliness requirement for incident response requiring real-time dependency information.

**See also:** Data Quality Dimension

#### Total Cost of Ownership

A comprehensive financial estimate including all direct and indirect costs of acquiring, deploying, operating, and maintaining an asset over its lifetime.

**Example:** The total cost of ownership for the relational CMDB includes licenses, hardware, maintenance, and 2 FTE for data quality management.

**See also:** TCO, Return on Investment

#### Transitive Dependency

An indirect dependency where component A depends on B, and B depends on C, implying A transitively depends on C.

**Example:** If the web application depends on the API service, which depends on the database, the web application has a transitive dependency on the database.

**See also:** Multi-Hop Query, Dependency Chain

#### Undirected Graph

A graph structure where edges have no specific direction and represent symmetric bidirectional relationships.

**Example:** In a network topology graph, undirected edges represent physical cable connections that function in both directions.

**See also:** Directed Graph

#### Upstream Dependency

A component or service that the current component depends on, which if failed would impact the current component's operation.

**Example:** The database is an upstream dependency of the application; if the database fails, the application cannot function.

**See also:** Downstream Dependency, Dependency Tracing

#### Validation Rule

A defined condition or constraint that data must satisfy to be considered acceptable.

**Example:** A validation rule requires that all server configuration items must have a valid IP address and operating system specified.

**See also:** Data Validation, Business Rule

#### Validity

A data quality dimension measuring whether data values conform to defined formats, ranges, and domain constraints.

**Example:** An IP address field containing "abc.def.xyz" fails validity checks because it doesn't match the required format.

**See also:** Data Quality Dimension, Data Validation

#### Vendor Evaluation

The systematic assessment of potential technology or service providers against organizational requirements and selection criteria.

**Example:** Vendor evaluation compared five CMDB solutions across criteria including graph capabilities, API quality, and total cost.

**See also:** Technology Selection, Vendor Management

#### Vendor Management

The practices and processes for selecting, contracting with, overseeing, and optimizing relationships with external service and technology providers.

**Example:** Vendor management ensures ServiceNow delivers contracted CMDB functionality and meets service level agreements.

**See also:** Vendor Evaluation

#### Vertex

An alternative term from graph theory for a node, representing a point in a graph structure.

**Example:** In graph theory literature, vertices are connected by edges to form graph structures.

**See also:** Node, Edge, Graph Theory

#### Vertical Scaling

Increasing system capacity by upgrading existing hardware with more powerful components rather than adding more machines.

**Example:** Vertical scaling upgrades the database server from 64GB to 256GB RAM instead of adding more database servers.

**See also:** Horizontal Scaling, Scalability

---

**Total Terms:** 200
**Generated:** 2025
**Standard:** ISO 11179 Metadata Registry Guidelines
