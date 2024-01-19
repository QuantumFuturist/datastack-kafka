# Kafka Cluster Setup with Docker Compose

[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://github.com/QuantumFuturist/datastack-kafka/blob/main/LICENSE)
---

#### Introduction
This repository contains a comprehensive Docker Compose setup for deploying a Kafka cluster along with its supporting services. It is designed to provide a robust, scalable, and easily understandable Kafka environment suitable for development, testing, and potentially for smaller production deployments.

#### Services Included:
1. **ZooKeeper**: Manages Kafka cluster metadata and coordination.
2. **Kafka Broker**: Core service for storing and processing messages.
3. **Kafka Connect**: Enables integration of Kafka with external data sources and sinks.
4. **Schema Registry**: Manages Avro schemas for Kafka messages, ensuring compatibility.
5. **KSQLDB Server and CLI**: Stream processing engine to process Kafka data in real-time.
6. **Kafka REST Proxy**: Provides a RESTful interface to the Kafka cluster.
7. **Kafka UI**: This project uses [Kafka-UI by provectus](https://github.com/provectus/kafka-ui) for Kafka management and monitoring.

#### Features:
- **Ease of Deployment**: One-command deployment of a full Kafka stack.
- **Scalability**: Easy to scale Kafka brokers and other components.
- **Configuration Customization**: Configuration options are externalized for easy customization.
- **Development and Testing**: Ideal environment for Kafka development and testing.
- **Health Checks**: Built-in health checks for service stability and monitoring.
- **Data Persistence**: Volumes configured for data persistence.

#### Best Practices Incorporated:
- **Service Dependencies**: Correct order and dependencies of services ensure smooth startup and operation.
- **Configuration Management**: Environment variables and external configuration files for easy management.
- **Network Configuration**: Custom network settings for inter-service communication.
- **Security**: Basic security configurations, with scope for further enhancements.
- **Monitoring and Logging**: JMX configuration for Kafka Broker monitoring.

#### Getting Started:
1. Clone the repository.
2. Navigate to the repository directory.
3. Run `docker compose up -d` to start all services.
4. Access Kafka UI at `http://localhost:8080` for cluster management.

#### Prerequisites:
- Docker and Docker Compose installed on your machine.
- Basic understanding of Kafka and Docker.

#### Customization:
- Modify the `.env` file for environment-specific settings.
- Update Docker Compose file for advanced configurations such as scaling brokers, adding more ZooKeeper nodes, etc.

#### Contributing:
Contributions to enhance this setup are welcome! Please adhere to the following guidelines:
- Fork the repository.
- Create a new branch for your feature.
- Open a pull request with a detailed description of your changes.

#### Disclaimer:
This setup is primarily for development and testing purposes. For production environments, additional configurations for security, high availability, and performance tuning are recommended.

---

*Feel free to open issues for any questions or suggestions regarding this Kafka Docker Compose setup.*