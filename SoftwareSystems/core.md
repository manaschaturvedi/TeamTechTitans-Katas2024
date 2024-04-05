# Core Service for Fish Watch

***Core Service*** is the central component responsible for housing the core application logic, business rules, data processing, and backend functionalities within the Fish Watch system. It serves as the backbone of the system, orchestrating data flow, handling business operations, and ensuring overall system functionality.

Below is the high-level architecture view of ***Core Service*** in the Fish Watch system.

![Core Service Architecture](https://example.com/core-service-architecture.png)

## Component Details

| Component Name  | Component Description | Technology Choices |
| ------------- | ------------- | ------------- |
| ***Business Logic Layer***  | Layer for implementing core business logic, domain-specific rules, workflows, data transformations, and processing algorithms to support Fish Watch functionalities. | Python, Elixir |
| ***Data Access Layer***  | Layer for accessing and interacting with data stores, databases, external APIs, and data sources to retrieve, store, update, and manage data required by the Core Service. | ORM Frameworks, RESTful APIs, SQL Databases, Caching Layer (Redis) |
| ***Service APIs***  | APIs exposed by the Core Service for communication with other system components, external services, user interfaces, and integration points within the Fish Watch ecosystem. | RESTful APIs |
| ***Event Handling***  | Component for handling asynchronous events, messaging, event-driven architecture patterns, and event processing within the Core Service for real-time updates and data synchronization. | RabbitMQ, Event-Driven Architecture |
| ***Security and Authentication***  | Security layer for implementing authentication, authorization, identity management, encryption, access control, and security policies to protect sensitive data and system resources. | OAuth2, JWT, SSL/TLS, Identity Providers |

### Component Diagram
![Core Component Diagram](../Assets/components/Core.svg)
<!-- ![Core Security Component Diagram](../Assets/components/Core-security.png) -->
<img src="../Assets/components/Core-security.png" alt="drawing" width="200"/>

## Architectural Characteristics

| Characteristics  | Decisions |
| ------------- | ------------- |
| Modularity  | Design the Core Service as a modular, decoupled architecture with well-defined boundaries, separation of concerns, and reusable components for scalability and maintainability. |
| Scalability  | Implement scalable architecture patterns such as microservices, distributed computing, horizontal scaling, and load balancing to handle growing system demands and user traffic. |
| Reliability  | Ensure high availability, fault tolerance, error handling, and recovery mechanisms within the Core Service to minimize downtime, data loss, and system failures. |
| Performance  | Optimize performance through efficient algorithms, caching strategies, database optimizations, asynchronous processing, and resource utilization monitoring for responsive system behavior. |

## Architectural Choice

- Microservices Architecture for modular, independent services, API-driven interactions, and agile development, deployment, and scaling of Core Service components.

## Deployment View
Below is the deployment view based on the architecture choice and this ADR [Deploy Core Service in cloud.md](../ADRs/014-deployment-strategy.md)

![Core Service Deployment View](../Assets/deployment/Core.png)
