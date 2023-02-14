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