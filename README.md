**Real-Time Stock Market Data Pipeline with Apache Kafka, Python & Cassandra on AWS EC2**
**Project Overview**
This project demonstrates a real-time data pipeline that captures live stock market data using Python, streams it through Apache Kafka deployed on an AWS EC2 instance, and stores the data into Apache Cassandra for persistence. It is designed for low-latency, high-throughput, and scalable ingestion of financial data.

**Key Features**
Data Engineering: Implements an end-to-end streaming pipeline for real-time data.

Technology Stack: Python, Apache Kafka, CassandraDB, AWS EC2.

Cloud Integration: Kafka is deployed on AWS EC2 for flexibility and scalability.

Resilience: Includes error handling for common integration issues.

Extendability: Allows future integration of ML models, dashboards, and alerts.

**Architecture**==
csharp
Copy
Edit
[Stock API] 
   ↓ 
[Python Producer (EC2)]
   ↓ 
[Kafka Broker (EC2)]
   ↓ 
[Python Consumer (EC2)]
   ↓ 
[CassandraDB (Local)]
🖥️ Environment Setup
🏠 Local Machine
OS: Ubuntu 22.04.1 LTS

Specs: 4 vCPUs, 4 GB RAM, 32 GB Disk

Role: Hosts Apache Cassandra

** AWS EC2**
OS: Amazon Linux 2 (Kernel 5.10)

Instance Type: t2.micro

Role: Runs Kafka broker, producer, and consumer scripts

**Prerequisites**
Install the following on relevant environments:

Python 3.x

kafka-python

cassandra-driver

Apache Kafka

Apache Cassandra

Java (JDK)

AWS CLI

🚀 **Implementation Steps**
Provision EC2 Instance

Launch EC2 using Amazon Linux 2

Install Java and Apache Kafka

Configure firewall (open port 9092)

Kafka Producer (Python)

Fetch stock market data from an API

Send it to Kafka topic using kafka-python

Kafka Broker

Start Zookeeper and Kafka server

Create a topic (e.g., stock_data)

Kafka Consumer (Python)

Consume data from the Kafka topic

Write data into Cassandra using cassandra-driver

Cassandra DB

Create keyspace and tables

Use CQL to validate data writes

🛠️ Execution Steps
Start Kafka on EC2

Run producer script to publish data

Run consumer script to save data to Cassandra

Query Cassandra with CQL to verify results

**❗ Error Handling & Troubleshooting
Issue	Resolution**
Kafka connection refused	Ensure Kafka is running on EC2 and port 9092 is open
Cassandra not reachable	Confirm Cassandra is running locally and listening on correct port
No data in topic	Check producer script and API connection
Insert error in Cassandra	Verify table schema matches the data format
Query errors	Use correct keyspace and ensure table exists

🔮 Project Overview
This project demonstrates a real-time data pipeline that captures live stock market data using Python, streams it through Apache Kafka deployed on an AWS EC2 instance, and stores the data into Apache Cassandra for persistence. It is designed for low-latency, high-throughput, and scalable ingestion of financial data.

🔧 Key Features
Data Engineering: Implements an end-to-end streaming pipeline for real-time data.

Technology Stack: Python, Apache Kafka, CassandraDB, AWS EC2.

Cloud Integration: Kafka is deployed on AWS EC2 for flexibility and scalability.

Resilience: Includes error handling for common integration issues.

Extendability: Allows future integration of ML models, dashboards, and alerts.

🧱 Architecture
csharp
Copy
Edit
[Stock API] 
   ↓ 
[Python Producer (EC2)]
   ↓ 
[Kafka Broker (EC2)]
   ↓ 
[Python Consumer (EC2)]
   ↓ 
[CassandraDB (Local)]
🖥️ Environment Setup
🏠 Local Machine
OS: Ubuntu 22.04.1 LTS

Specs: 4 vCPUs, 4 GB RAM, 32 GB Disk

Role: Hosts Apache Cassandra

☁️ AWS EC2
OS: Amazon Linux 2 (Kernel 5.10)

Instance Type: t2.micro

Role: Runs Kafka broker, producer, and consumer scripts

📦 Prerequisites
Install the following on relevant environments:

Python 3.x

kafka-python

cassandra-driver

Apache Kafka

Apache Cassandra

Java (JDK)

AWS CLI

🚀 Implementation Steps
Provision EC2 Instance

Launch EC2 using Amazon Linux 2

Install Java and Apache Kafka

Configure firewall (open port 9092)

Kafka Producer (Python)

Fetch stock market data from an API

Send it to Kafka topic using kafka-python

Kafka Broker

Start Zookeeper and Kafka server

Create a topic (e.g., stock_data)

Kafka Consumer (Python)

Consume data from the Kafka topic

Write data into Cassandra using cassandra-driver

Cassandra DB

Create keyspace and tables

Use CQL to validate data writes

🛠️ Execution Steps
Start Kafka on EC2

Run producer script to publish data

Run consumer script to save data to Cassandra

Query Cassandra with CQL to verify results

❗** Error Handling & Troubleshooting
Issue	Resolution**
Kafka connection refused	Ensure Kafka is running on EC2 and port 9092 is open
Cassandra not reachable	Confirm Cassandra is running locally and listening on correct port
No data in topic	Check producer script and API connection
Insert error in Cassandra	Verify table schema matches the data format
Query errors	Use correct keyspace and ensure table exists

 Project Overview
This project demonstrates a real-time data pipeline that captures live stock market data using Python, streams it through Apache Kafka deployed on an AWS EC2 instance, and stores the data into Apache Cassandra for persistence. It is designed for low-latency, high-throughput, and scalable ingestion of financial data.

🔧 Key Features
Data Engineering: Implements an end-to-end streaming pipeline for real-time data.

Technology Stack: Python, Apache Kafka, CassandraDB, AWS EC2.

Cloud Integration: Kafka is deployed on AWS EC2 for flexibility and scalability.

Resilience: Includes error handling for common integration issues.

Extendability: Allows future integration of ML models, dashboards, and alerts.

🧱 Architecture
csharp
Copy
Edit
[Stock API] 
   ↓ 
[Python Producer (EC2)]
   ↓ 
[Kafka Broker (EC2)]
   ↓ 
[Python Consumer (EC2)]
   ↓ 
[CassandraDB (Local)]
🖥️ Environment Setup
🏠 Local Machine
OS: Ubuntu 22.04.1 LTS

Specs: 4 vCPUs, 4 GB RAM, 32 GB Disk

Role: Hosts Apache Cassandra

☁️ AWS EC2
OS: Amazon Linux 2 (Kernel 5.10)

Instance Type: t2.micro

Role: Runs Kafka broker, producer, and consumer scripts

📦 Prerequisites
Install the following on relevant environments:

Python 3.x

kafka-python

cassandra-driver

Apache Kafka

Apache Cassandra

Java (JDK)

AWS CLI

🚀 Implementation Steps
Provision EC2 Instance

Launch EC2 using Amazon Linux 2

Install Java and Apache Kafka

Configure firewall (open port 9092)

Kafka Producer (Python)

Fetch stock market data from an API

Send it to Kafka topic using kafka-python

Kafka Broker

Start Zookeeper and Kafka server

Create a topic (e.g., stock_data)

Kafka Consumer (Python)

Consume data from the Kafka topic

Write data into Cassandra using cassandra-driver

Cassandra DB

Create keyspace and tables

Use CQL to validate data writes

🛠️ Execution Steps
Start Kafka on EC2

Run producer script to publish data

Run consumer script to save data to Cassandra

Query Cassandra with CQL to verify results
Query errors	Use correct keyspace and ensure table exists

** **Future Enhancements****
Visualization: Use Seaborn/Matplotlib to plot stored market trends

Machine Learning: Forecast prices using regression or LSTM models

Real-Time Alerts: Send email/SMS on sudden price spikes or drops

Scalability: Add multiple Kafka brokers and Cassandra nodes for load distribution

Cloud Storage: Add support for AWS S3, Redshift, or Amazon Keyspaces

** **Conclusion****
This project integrates Python, Apache Kafka, AWS EC2, and CassandraDB to build a real-time, cloud-accelerated pipeline. It is scalable, flexible, and serves as a robust foundation for financial analytics, IoT telemetry, or time-series data system Future Enhancements
Visualization: Use Seaborn/Matplotlib to plot stored market trends

Machine Learning: Forecast prices using regression or LSTM models

Real-Time Alerts: Send email/SMS on sudden price spikes or drops

Scalability: Add multiple Kafka brokers and Cassandra nodes for load distribution

Cloud Storage: Add support for AWS S3, Redshift, or Amazon Keyspaces

🧾 Conclusion
This project integrates Python, Apache Kafka, AWS EC2, and CassandraDB to build a real-time, cloud-accelerated pipeline. It is scalable, flexible, and serves as a robust foundation for financial analytics, IoT telemetry, or time-series data systems.
Visualization: Use Seaborn/Matplotlib to plot stored market trends

Machine Learning: Forecast prices using regression or LSTM models

Real-Time Alerts: Send email/SMS on sudden price spikes or drops

Scalability: Add multiple Kafka brokers and Cassandra nodes for load distribution

Cloud Storage: Add support for AWS S3, Redshift, or Amazon Keyspaces

🧾 Conclusion
This project integrates Python, Apache Kafka, AWS EC2, and CassandraDB to build a real-time, cloud-accelerated pipeline. It is scalable, flexible, and serves as a robust foundation for financial analytics, IoT telemetry, or time-series data systems.
