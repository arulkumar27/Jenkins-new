# Jenkins Architecture

## Overview

Jenkins follows a Master-Agent Architecture.

Components:

1. Jenkins Controller (Master)
2. Jenkins Agent (Node)

## Jenkins Controller

Responsible for:

- Scheduling Jobs
- Managing Builds
- Managing Agents
- User Authentication
- Plugin Management

## Jenkins Agent

Responsible for:

- Executing Builds
- Running Tests
- Deployment Tasks

## Architecture Diagram

Developer
↓
GitHub
↓
Jenkins Controller
↓
Agent Node
↓
Build
↓
Deploy

## Real-Time Scenario

Company has:

- 100 Developers
- 500 Builds Daily

Master cannot execute all builds.

Solution:

Master controls builds.

Agents execute builds.

Agents:
- Linux Agent
- Windows Agent
- Docker Agent

## Advantages

- Scalability
- Better Performance
- Faster Builds
- Load Distribution

## Interview Questions

Q: What are Jenkins Agents?

Answer:
Agents are worker machines that execute build jobs assigned by the Jenkins Controller.

Q: Why use Agents?

Answer:
To distribute workloads and improve build performance.
