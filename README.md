⚡ Apache Kafka Project

This repository contains an implementation of Apache Kafka, a distributed event streaming platform used for building real-time data pipelines and event-driven applications.



🚀 Features

🔄 Publish-subscribe messaging

🔥 High-throughput and fault-tolerant event streaming

🔧 Kafka producer and consumer implementation

🏎️ Scalable architecture

🛠 Tech Stack

Messaging System: Apache Kafka

Programming Language: Java / Python / Node.js (Specify your stack)

Broker Setup: Zookeeper + Kafka Brokers

Data Processing: Kafka Streams / Spark Streaming (if applicable)

📁 Project Structure


/Kafka

│── /producers        # Kafka producers (publishing messages)

│── /consumers        # Kafka consumers (subscribing messages)

│── /config           # Kafka configurations

│── /scripts          # Helper scripts for setup

│── docker-compose.yml # Kafka with Docker (if used)

│── README.md         # Documentation

🚀 Installation & Setup

1️⃣ Install Kafka (Local Setup)

Download and extract Kafka




wget https://downloads.apache.org/kafka/3.4.0/kafka_2.13-3.4.0.tgz

tar -xvzf kafka_2.13-3.4.0.tgz

cd kafka_2.13-3.4.0

Start Zookeeper & Kafka Broker





bin/zookeeper-server-start.sh config/zookeeper.properties

bin/kafka-server-start.sh config/server.properties

2️⃣ Create Kafka Topics


bin/kafka-topics.sh --create --topic test-topic --bootstrap-server localhost:9092 --partitions 3 --replication-factor 1

3️⃣ Start Producer & Consumer

Producer (Publishing Messages):





bin/kafka-console-producer.sh --topic test-topic --bootstrap-server localhost:9092

Consumer (Listening to Messages):




bin/kafka-console-consumer.sh --topic test-topic --from-beginning --bootstrap-server localhost:9092

🛠 Running with Docker (If Used)

docker-compose up -d

📌 Contributing

Contributions are welcome! Feel free to:

✅ Fork the repository

✅ Create a new branch

✅ Make changes and submit a pull request


