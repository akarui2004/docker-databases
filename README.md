# Docker Databases

A comprehensive Docker-based development environment for various databases and related services.

## Overview

This project provides a ready-to-use collection of database systems and cloud service emulators configured with Docker for local development. It includes relational databases, NoSQL databases, caching systems, message brokers, and monitoring tools.

## Services Included

### Relational Databases (RDS)
- **PostgreSQL** (v16)
  - Includes `uuid-ossp` extension
  - Configured with 1GB shared memory (shm_size)
- **MySQL 5.7**
  - Native password authentication
  - UTF-8 (utf8mb4) character set support
- **MySQL 8.0**
  - Native password authentication
  - UTF-8 (utf8mb4) character set support

### NoSQL Databases
- **MongoDB**

### Cache Systems
- **Redis** (v7.4)
  - Configured with cluster mode enabled

### AWS Stack
- **LocalStack** - for emulating AWS services (S3, SQS, SNS, Lambda, DynamoDB)
- **MinIO** - S3-compatible object storage

### Message Brokers
- **Kafka** with **Zookeeper**

### Monitoring
- **Datadog Agent**

## Prerequisites

- Docker and Docker Compose
- Git

## Quick Start

1. Clone the repository
2. Configure environment variables:
   ```bash
   cp .env.example .env
   # Edit .env file to customize settings
   ```
