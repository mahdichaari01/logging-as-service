# End of year project: Logging as a service

## Description

This project aims to provide a centralized logging solution as a service, enabling users to efficiently manage and analyze logs generated by various applications.

## Table of Contents

1. [Architecture](#architecture)
2. [Services and Tools](#services-and-tools)
3. [License](#license)

## Architecture

The logging service is designed with a microservices architecture, consisting of the following named components:

1. **Auth Service**: Responsible for authentication and authorization of clients. Manages user database and authentication mechanisms.

2. **WebSocket Service**: Handles real-time communication between client applications and the logging system, enabling instant log updates.

3. **Analytics Service**: Performs analysis on log data to generate insights, identify patterns, and detect anomalies.

4. **Frontend Service**: Provides a user-friendly web interface for interacting with the logging system, including log visualization and querying capabilities.

5. **gRPC logging Endpoint**: Offers a high-performance and language-agnostic communication protocol for client-server communication, providing efficient data transfer between services.

6. **Kafka Service**: Facilitates data replication and stream processing, ensuring fault tolerance and scalability in log processing.

7. **Persistence and Storage Service**: Manages storage and retrieval of log data, ensuring durability and efficient access.

Each service utilizes specific tools and technologies for its functionalities:

### Auth Service

- **Framework**: Flask
- **Database**: PostgreSQL
- **Authentication Mechanism**: JWT Tokens
- **User Database Management**: SQLAlchemy

### WebSocket Service

- **Framework**: Node.js with Socket.IO
- **Real-time Communication**: WebSockets
- **Event-driven Architecture**: Socket.IO Events

### Analytics Service

- **Framework**: Apache Spark
- **Machine Learning**: TensorFlow
- **Anomaly Detection**: Isolation Forest Algorithm
- **Data Processing**: Spark SQL

### Frontend Service

- **Framework**: React.js
- **Data Visualization**: D3.js
- **Backend Integration**: RESTful APIs

### Public gRPC Endpoint

- **Protocol**: gRPC
- **Efficient Communication**: Protocol Buffers
- **Inter-service Communication**: gRPC Server and Client

### Kafka Service

- **Distributed Messaging System**: Apache Kafka
- **Data Replication**: Kafka Replication
- **Stream Processing**: Kafka Streams API

### Persistence and Storage Service

- **Database**: Elasticsearch
- **Scalable Storage**: Elasticsearch Sharding
- **Indexing and Searching**: Elasticsearch Indexing API

This architecture ensures modularity, scalability, and fault tolerance in the logging system, allowing for efficient management and analysis of log data.

## License

This project is licensed under the [MIT License](LICENSE).

Certainly! Here's a revised architecture with named services:
