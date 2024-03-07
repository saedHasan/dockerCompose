# Instruction to Run docker compose file

# Step1: Create Docker Compose File
  Create a docker-compose.yml file in your project directory

# Step2: Create server.properties File
  Create a server.properties file containing SASL configurations for Kafka brokers. Place this file in the same directory as your docker- 
  compose.yml file

# Step3: Create server-jaas.conf File 
  Create a server-jaas.conf file containing JAAS configurations for SASL authentication. Place this file in the same directory as your 
  docker-compose.yml file.

# Step4: Start the Kafka Cluster
  Run below command: 

  ```bash
  docker-compose up -d
  ```
  
This command will start Zookeeper and three Kafka brokers (kafka1, kafka2, and kafka3) with SASL authentication enabled.

# Step5: Verify Kafka Cluster: 
  After the Kafka cluster is up and running, you can verify its status by connecting to one of the brokers and running Kafka commands, such 
  as creating topics or producing/consuming messages.

   ```bash
    docker ps
   ```
  This will list all the running process for zookeeper and kafka brokers.


# END 

