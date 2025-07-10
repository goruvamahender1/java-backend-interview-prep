## SpringBoot Intermediate Answers

---

#### 1.
Spring Boot provides built-in support using Spring Boot Actuator to expose metrics and health endpoints.
 For centralized logging and monitoring:
Use tools like the ELK stack (Elasticsearch, Logstash, Kibana).
Or Prometheus and Grafana for metrics and alerting.
Use Case Example:
 In production, instead of checking logs on each server, logs are sent to Elasticsearch and visualized in Kibana. This helps in tracking errors, request flows, and app performance from one place.