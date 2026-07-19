# Architecture

SprintSync follows a Modular Monolith Architecture.

Frontend and Backend are developed independently while remaining inside a single Git repository.

## Frontend

React

↓

TanStack Query

↓

Fetch API

↓

Spring Boot REST APIs

## Backend

Controller

↓

Service

↓

Repository

↓

PostgreSQL

The architecture is intentionally designed so that Docker, Redis, Kafka, Email Service, and Microservices can be introduced in future versions without major restructuring.