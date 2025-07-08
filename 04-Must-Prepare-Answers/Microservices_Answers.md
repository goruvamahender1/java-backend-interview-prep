## Microservices Must Prepare Answers

---

#### 12.

1️⃣ Service Registry & Discovery
=> Helps services find and communicate with each other dynamically.
🔧 Tools: Eureka, Consul

2️⃣ API Gateway
=> Acts as a single entry point, handling request routing, authentication, and load balancing.
🔧 Tools: Zuul, Spring Cloud Gateway

3️⃣ Circuit Breaker
=> Prevents system-wide failures by cutting off requests to struggling services.
🔧 Tools: Resilience4j, Hystrix

4️⃣ Database Per Service
=> Each microservice gets its own database to maintain data isolation and prevent tight coupling.

5️⃣ Saga Pattern
=> Manages distributed transactions across multiple services via orchestration or choreography.
🔧 Tools: Camunda, Temporal

6️⃣ Strangler Fig Pattern
=> A safe way to migrate from a monolith to microservices—gradually replacing pieces instead of a risky big bang rewrite.

7️⃣ Event Sourcing
=> Stores every state change as an event, allowing for historical tracking and easier debugging.

8️⃣ CQRS (Command Query Responsibility Segregation)
=> Separates read and write operations for better scalability and performance.

9️⃣ Sidecar Pattern
=> Adds extra capabilities like logging, monitoring, or security without changing the main service.
🔧 Tools: Istio, Envoy

🔟 Publish-Subscribe (Pub-Sub)
=> Services communicate asynchronously, ensuring loose coupling and better scalability.
🔧 Tools: Kafka, RabbitMQ