# Carrer Roadmap

#[Pattern's Literature](https://github.com/AriTedeschi/AriTedeschi/edit/main/Roadmap/RoadMap.md "Pattern's Literature")

#[Data Management](https://github.com/AriTedeschi/AriTedeschi/edit/main/Roadmap/RoadMap.md "Data Management")

#[DevOps](https://github.com/AriTedeschi/AriTedeschi/edit/main/Roadmap/RoadMap.md "DevOps")

#[Tips for API Security](https://github.com/AriTedeschi/AriTedeschi/edit/main/Roadmap/RoadMap.md "Tips for API Security")


**IMPORTANT:**
Create a Template to a Brag Document

Design Patterns:
- [x] MVC;
- [x] Builder;
- [x] Repository;
- [ ] Mediator;
- [ ] CQRS;
- [ ] Event Sourcing;
- [x] Factory;
- [x] Facade;
- [x] Strategy;
- [ ] Transporter;

Java Libraries and Priciples:
- [ ] Quarkus;
- [x] Rest Maturity Levels;
- [ ]  Principles
	 - [ ] SOLID;
	 - [ ] DRY;
	 - [ ] YAGNI;
	 - [ ] KISS;
	 - [ ] Clean Code (top 7);

## Architecture
Domain-driven design:
- [ ] Ubiquitous Language 
- [ ] Domain;
- [ ] Bounded Context;
- [ ] Map;
- [ ] Models;
- [ ] Aggregate;
- [ ] Domain Services;
- [ ] Repositories;

Microservices:
- [ ] Logging;
- [ ] Module;
- [ ] Back-end for Front-end;
- [ ] Autoscale

## Data Management
Relational Database:
- [x] Postgres
- [x] Mysql
- [x] Sql Server
- [x] Oracle Database

Non-relational Databases:
- [ ] Redis;
- [ ] MondoDB;
- [ ] Elastic Search;

Queues:
- [X] RabbitMQ;
- [ ] Kafka;
- [ ] Pulsar;

## DevOps
 CI/CD:
 - [x] Github;
 - [x] Gitflow;
 - [x] Jenkins;
 - [x] Docker:
	 - [x] Docker File;
	 - [x] Docker HUB;
	 - [x] Docker Compose;
 - [ ] Kubernetes;
 - [ ] OpenShift;
 - [ ] Rundeck.
 
 Infrastructure:
- [ ] Forward Proxy;
- [ ] Reverse Proxy;

Infrastructure as Code:
- [ ] Serveless;
- [ ] Cloudformation;
- [ ] Terraform;
- [ ] Ansible;

Cloud Providers:
- [x] Azure;
- [x] Oracle Cloud Infrastructure;
- [ ] Google Cloud Plataform;
- [ ] Amazon Web Services
	 - [ ] API Gateway;
	 - [ ] SQS;
	 - [ ] SNS;
	 - [ ] LAMBDA;
	 - [ ] DYNAMODB;
	 - [ ] S3;
	 - [ ] EC2;
	 - [ ] RDS;
	 - [ ] GLUE;
	 - [ ] EKS;
	 - [ ] ECS;
	 - [ ] CLOUDWATCH;
	 - [ ] KINESIS;
	 - [ ] QUICKSIGHT;
	 - [ ] CODEBUILD;

Monitoring/Observability:
- [x] Sonarqube;
- [ ] Grafana;
- [ ] Kibana;
- [ ] Datadog;
- [ ] New Relic;
- [ ] OpsGenie;
- [ ] Sentry;

Mobile testing:
- [ ] Fastlane;
- [ ] Codemagic;
- [ ] Bitrise;

Web testing:
- [ ] Robot Framework

## Pattern's Literature
### Design Patterns for Microservices:
- [ ]  Observability Patterns: Learn About the inner workings of your microservices, ensuring system health and performance.  
	 - Log Aggregation;
	 - Performance Metrics;
	 - Distributed Tracing;
	 - Health Check;
- [ ] Database Patterns: Optimize data management for microservices, considering data ownership, consistency, and scalability.  
	 - Shared Database per Service;
	 - Database per Service;
	 - CQRS;
	 -  Event Sourcing;
	 - Saga Pattern;
- [ ] Integration Patterns: Establish seamless communication between microservices, enabling efficient data exchange.  
	 - API Gateway;
	 - Aggregator Pattern;
	 - Proxy Pattern;
	 - Client-side UI Composition Pattern;
	 - Branched Pattern;
	 - Chained Microservice Pattern;
	 - Gateway Routing Pattern;
- [ ] Decomposition Patterns: Break down complex functionalities into well-defined, independent microservices, promoting maintainability and scalability.  
	 - Decompose by Business Capability;
	 - Decompose by Subdomain;
	 - Decompose by Transactions;
	 - Strangler Pattern;
	 - Bulkhead Pattern;
	 - Sidecar Pattern;
- [ ] Cross-Cutting Concern Patterns: Address concerns like security, logging, and authentication consistently across your microservices.
	 - External Configuration;
	 - Service Discovery Pattern
	 - Circuit Breaker Pattern
	 - Blue-green Deployment Pattern

### Authentication Methods on REST API:
- Basic Authentication;
- Token Authentication;
- OAuth Authentication;
- API Key Authentication;
- Single Sign-On;

### Tips for API Security  
- Use HTTPS  
- Use OAuth2  
- Use WebAuthn  
- Use Leveled API Keys  
- Authorization  
- Rate Limiting  
- API Versioning  
- Whitelisting  
- Check OWASP API Security Risks  
- Use API Gateway  
- Error Handling  
- Input Validation

https://www.localstack.cloud/

https://dly.to

### Cloud Messaging Patterns
🔹 Asynchronous Request-Reply  
This pattern aims at providing determinism for long-running backend tasks. It decouples backend processing from frontend clients.
🔹 Publisher-Subscriber  
This pattern targets decoupling senders from consumers, and avoiding blocking the sender to wait for a response.
🔹 Claim Check  
This pattern solves the transmision of large messages. It stores the whole message payload into a database and transmits only the reference to the message, which will be used later to retrieve the payload from the database.
🔹 Priority Queue  
This pattern prioritizes requests sent to services so that requests with a higher priority are received and processed more quickly than those with a lower priority.
🔹 Saga  
Saga is used to manage data consistency across multiple services in distributed systems, especially in microservices architectures where each service manages its own database.
🔹 Competing Consumers  
This pattern enables multiple concurrent consumers to process messages received on the same messaging channel. There is no need to configure complex coordination between the consumers. However, this pattern cannot guarantee message ordering.

