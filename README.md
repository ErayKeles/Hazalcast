# Hazelcast-Based Telecommunication Management System (EntroCell)

## Overview
The **Telecommunication Management System (OCS)** is a robust and scalable application designed to manage telecommunication operations efficiently. Built with **Kafka**, **Docker**, **Hazelcast**, and **Oracle**, this project leverages distributed systems and cloud-based deployment to handle large-scale data and real-time operations seamlessly.

## Features
- **Distributed Data Management**: Utilizes Hazelcast for efficient and fault-tolerant distributed data operations.
- **Cloud Deployment**: Fully containerized and deployable using Docker.
- **Middleware Integration**: Provides middleware capabilities using Hazelcast MW Operations.
- **Real-Time Simulation**: Includes a simulator to test and validate operations in real-time.

## Project Structure
```
Hazelcast_EnteroCELL-main
│
├── pom.xml                     # Maven build configuration
├── src/main/java/org/example
│   ├── Main.java               # Entry point of the application
│   ├── hazelcast_operations
│   │   ├── HazelcastDGWOperation.java  # Data Gateway Operations
│   │   ├── HazelcastMWOperation.java   # Middleware Operations
│   │   ├── HazelcastSimulatorOperation.java  # Simulator Operations
│   ├── utils
│       ├── configurations
│       │   ├── Configuration.java      # Application Configurations
│       ├── constants
│           ├── StringConstants.java    # String Constants
│
├── target/classes              # Compiled Java classes
```

## Technologies Used
- **Hazelcast**: For distributed data caching and real-time computations.
- **Kafka**: Message streaming platform for handling event-driven architecture.
- **Docker**: For containerization and cloud deployments.
- **Oracle Database**: Backend for data persistence and management.
- **Java**: Core programming language for building the application.
- **Maven**: Build and dependency management.

## Getting Started

### Prerequisites
Ensure you have the following tools installed:
- **Java JDK 11+**
- **Apache Maven**
- **Docker**
- **Oracle Database** (or a compatible database service)

### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/Hazelcast_EnteroCELL.git
   cd Hazelcast_EnteroCELL-main
   ```

2. Build the project:
   ```bash
   mvn clean install
   ```

3. Run Docker to set up the required services (Kafka, Hazelcast, etc.):
   ```bash
   docker-compose up -d
   ```

4. Run the application:
   ```bash
   java -jar target/Hazelcast_EnteroCELL.jar
   ```

### Configuration
Modify the `Configuration.java` file to set your environment variables, including:
- Kafka broker URLs
- Database connection strings
- Hazelcast cluster settings

## Usage
- **Simulate Operations**: Use the `HazelcastSimulatorOperation` class to simulate and validate real-time telecommunication operations.
- **Middleware Tasks**: Execute middleware operations using the `HazelcastMWOperation` class.
- **Data Gateway**: Manage distributed data tasks with `HazelcastDGWOperation`.

## Contribution
Contributions are welcome! Please follow these steps:
1. Fork the repository.
2. Create a feature branch (`git checkout -b feature-name`).
3. Commit your changes (`git commit -m 'Add feature'`).
4. Push to the branch (`git push origin feature-name`).
5. Open a Pull Request.

## License
This project is licensed under the MIT License. See the `LICENSE` file for details.

## Contact
For any inquiries or feedback, feel free to reach out:
- **Email**: eraykelesk@gmail.com
- **LinkedIn**: [Eray Keleş](https://linkedin.com/in/eraykeles)
