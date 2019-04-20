# Microchestrator (version 0.1.0)
This is an implementation of Saga pattern for microservices and IoT devices. It focuses on serving as a lightweight and high performance hybrid, between Choreography-based and Orchestration-based, service. The service's user can configure Microchestrator through the content of registration.json and orchestration.json files for best suit its purpose in a project.

The architecture diagram below illustrates the relationship between Microchestrator and external microservices and IoT devices:

![Microchestrator Architecture](docs/microchestrator_architecture.png)

**Orchestration Topics:** A topic is a collection of events and the associated actions/callbacks of microservices.

**Topic States:** A topic state keeps the status of defined action(s) within a topic.

**Event States:** An event state holds the status of a specific event. It has three possible states - pending, completed and failed.

**Event Microservice:** This microservice offers an interface to those external entities who do not have access to event channels.

**Event Broker:** An event broker that supports industrial standard communication protocol such as MQTT and STOMP.

