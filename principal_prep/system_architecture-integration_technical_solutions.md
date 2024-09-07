safety much be shown not assumed

## Infeasibility of Complete Testing

Building a fleet of vehicles big enough to run billions of hours is impactical

## V model as a starting point

## Driver out of the loop
### Controllability Challenges
Situations where driver does not have an ability to take correctvie action are said to lack controllability and must be designed to a higher Automotive Safety Integrity Level (ASIL).

Computer system must assume the role as the primary exception handler for faults, malfunctions and beyond-specified operating conditions.

Fully AV must have significant additional complexity to deal with all the ways things might go wrong.

## Autonoomy Architecture Approaches
A monitor / actuator architecture

Regardless of the approach, there must be a way to detect when autonomy functions are not working properly and to bring the system to a safe state


## Complex Requirements

V model - the assumptions are that the requirements are actually known, correct, complete, and unambiguously specified.

### Requirements Challenges

The combination of adverse events and driving conditions are too numerous to enumerate in the classical written requirements specification.

It is unlikely that a classical V process that starts with a document that enumerates all system requirements will be scalable to scalable to AV exception handling in a rigorous way.

### Operational Concept Approaches
Constrain operational concepts and engage in a phased expansion of requirements.

Mitigation of requirement complexity can be achieved via only enabling autonomy in a certain limited set of situations for which requirements are fully understood

### Safety Requirements and Invariants
Create a separate, parallel set of requirements that are strictly safety related.

* Non-safety related functional requirements (traditional and ML)
  * Can be mapped to low ASIL actuator functions
* Safety requirements
  * high ASIL monitor

## Non-deterministic and Statistical Algorithms
Statistical technologies tend to be non-deterministic in nature

### Challenges of Stochastic Systems
Every vehicle-level test could potentially result in a different outcome despite attempts to exercise nominally identically test cases

Uncertain sensor readings
Probabilistic perception algorithms
A tradeoff between false negative and false positive

### Non-determinism in Testing
* Difficult to exercise a particular edge-case situation
* Difficult to eval whether the test results are correct or not - there is no unique correct system behavior for a given test case.
  * test passes if the end system state is within an acceptabe 'test pass' envelop.

## Machine Learning Systems
* training examples are used to derive a model - inductive learning
* how to validate the ML systems? It makes it difficult to predict how techniques can be apply for ML system validation other than brute force testing
* black swan problem - if there is a special case the system has not seen, it cannot learn that case.


## Mission Critical Operational Requirements
* fail operational system design
  * component redundancy (VIC1 / VIC2) - need at least three




  

