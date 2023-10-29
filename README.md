# E Commerce

## Requirements to run the project

- Java 11 temurin
- Maven
- mongodb
- postgres
- redis
- RabbitMQ
- ElasticSearch
- logstash
- kibana
- nginx

| Service        | Port                   |
| -------------- | ---------------------- |
| postgres       | 5432                   |
| MongoDB        | 27017                  |
| RabbitMQ       | 5672/15672             |
| Redis          | 6379                   |
| Elastic Search | 9200/9300              |
| Logstash       | 4560, 4561, 4562, 4563 |
| Kibana         | 5601                   |
| Nginx          | 80                     |
| ECom-app       | 8080                   |
| ECom-search    | 8081                   |
| ECom-admin     | 8082                   |

## Preparing the environment to run the project

### 1. Install Java 11

```bash
sudo apt install openjdk-11-jdk
```

### 2. Install Maven

```bash
sudo apt install maven
```

### 3. Install Postgres

```bash
sudo apt install postgresql postgresql-contrib
```

### 4. Install MongoDB

```bash
sudo apt install mongodb
```

### 5. Install Redis

```bash
sudo apt install redis-server
```

### 6. Install RabbitMQ

```bash
sudo apt install rabbitmq-server
```

### 7. Install ElasticSearch

```bash
sudo apt install elasticsearch
```

### 8. Install Logstash

```bash
sudo apt install logstash
```

### 9. Install Kibana

```bash
sudo apt install kibana
```

### 10. Install Nginx

```bash
sudo apt install nginx
```

## Running the project

### 1. Start Postgres

```bash
sudo service postgresql start
```

### 2. Start MongoDB

```bash
sudo service mongodb start
```

### 3. Start Redis

```bash
sudo service redis-server start
```

### 4. Start RabbitMQ

```bash
sudo service rabbitmq-server start
```

### 5. Start ElasticSearch

```bash
sudo service elasticsearch start
```

### 6. Start Logstash

```bash
sudo service logstash start
```

### 7. Start Kibana

```bash
sudo service kibana start
```

### 8. Start Nginx

```bash
sudo service nginx start
```

> Note: Get the nginx.conf file from the project 'document/nginx/nginx.conf' and replace the default nginx.conf file with it.

### 9. Start ECom-app

```bash
cd ECom-app
mvn install
mvn package
java -jar target/*.jar
```

### 10. Start ECom-search

```bash
cd ECom-search
mvn install
mvn package
java -jar target/*.jar
```

### 11. Start ECom-admin

```bash
cd ECom-admin
mvn install
mvn package
java -jar target/*.jar
```
