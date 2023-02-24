# Designing Data-Intensive Applications

## Week 2

### Chapter 1 Reliable, Scalable, and Maintainable Applications

#### Reliablility

- Hardware Faults
- Software Errors
- Human Errors

From hardware to human, the possibility of problems is more likely to happen. So, reliability is not just for nuclear, but everywhere. We need to consider more when the application closes to people.



#### Scalability

Scalability is how we improve performance to cope with increasing load.

- Load: requestes/minutes.
- Performance: percentile is a better way to measure it.

##### How to scale?

- Scaling up or *vertical scaling*: more **powerful** machine.

- Scaling out or *horizontal scaling*: more **machines**.

Think about a comination of them

##### Pros and Cons of Elastic

* Pro: automatically add computing resources.
* Con: unpredictable, more surprises.




#### Maintainability

The core thingking about maintainability is all about how you deal with human:

- Operability: Easy for **Operation teams**
- Simplicity: Easy for **New engineers**

Abstraction is the best tool for removing accidental complexity.

- Evolvability: Easy for **Engineers to Change**



### Chapter 2 Data Models and Query Languages



#### Relational Model Versus Document Model

##### Relational Model

SQL, use tables, columns, and rows to present the data structure.

##### Document Model

NoSQL, more like an object-oriented data model.

##### The Object-Relational Mismatch

The structure of the object-oriented data is like a tree, but the relational data only contains tables, columns, and rows. The data transformation always need a join operation.

##### Debate

The relational model databases dominate the contemporary computer era, notwithstanding the document model databases regularly revived. When we choose a database type, we must consider the trio of the creeds: reliability, scalability, and maintainability.



#### Query Languages for Data

- Declarative: describe the data you want, more like a filter.
- Imperative: describe the procedure to make the data, more like use a basket pick the data you want.

*From a rudimentary perspective, declarative languages are not necessarily better than imperative languages. However, due to the abstract layer of declarative languages, they can reduce the inefficiency of poorly written imperative code, which can indirectly improve performance.*

- MapReduce: a combination of declarative query and imperative query.



#### Graph-Like Data Models
##### Property Graphs
- Vertex: identifier, two set of different edges, a map of properties
- Edge: identifier, two vertices it connected, a lable to describe the relations, a map of properties

Graph-like data models have the most flexibility, **is there any bad side?**
##### The Cypher Query Language
