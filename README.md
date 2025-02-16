# Distributed E-Commerce Platform with Shared Shopping Cart

## Overview
The **Distributed E-Commerce Platform with Shared Shopping Cart** is a microservices-based architecture designed to enhance online shopping experiences with seamless scalability, high availability, and efficient performance.

## Features
- **Microservices Architecture**: Modular services for user sessions, product catalog, shopping cart, activity logs, and recommendations.
- **Shared Shopping Cart**: Allows users to collaboratively add, update, and purchase items.
- **Containerized Deployment**: Uses **Docker** and **AWS ECS** for initial deployment, later optimized for **Kubernetes (EKS)**.
- **Service Discovery & Load Balancing**: Implemented via **Kubernetes Ingress** and **AWS ALB** for traffic management.
- **Performance Optimization**: 
  - **20% Faster API Responses** via **Redis Caching** and **MongoDB Query Optimization**.
  - **Event-Driven Architecture** with **Kafka** for real-time activity tracking and personalized recommendations.
- **Scalability & Fault Tolerance**:
  - Self-healing and rolling updates with **Kubernetes**.
  - Message queues ensure data consistency and fault recovery.

## Technologies Used
- **Backend**: Golang, REST API
- **Database**: MongoDB, Redis (for caching)
- **Infrastructure**: Kubernetes (EKS), Docker, AWS ECS
- **Messaging & Streaming**: Kafka (for event-driven architecture)
- **Frontend**: JavaScript (for UI interactions)

## System Architecture
The platform consists of multiple independent services:
- **User Service**: Manages authentication and session handling.
- **Product Service**: Maintains the product catalog.
- **Shopping Cart Service**: Enables shared cart functionality across users.
- **Order & Payment Service**: Handles order processing and payments.
- **Logging & Analytics Service**: Tracks user activity and system logs.
- **Recommendation Engine**: Provides personalized product recommendations.
