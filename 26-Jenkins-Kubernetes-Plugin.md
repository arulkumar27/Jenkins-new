# Jenkins Kubernetes Plugin

## What is Kubernetes Plugin?

Allows Jenkins to dynamically create Kubernetes Pods for builds.

Instead of static agents, Jenkins creates temporary build agents.

## Workflow

Jenkins
↓
Kubernetes Plugin
↓
Pod Created
↓
Build Runs
↓
Pod Deleted

## Benefits

- Scalability
- Cost Optimization
- Resource Efficiency

## Installation

Manage Jenkins
↓
Plugins
↓
Kubernetes Plugin

## Real-Time Scenario

100 builds start simultaneously.

Kubernetes automatically creates required build pods.

## Interview Question

Q: Why use Kubernetes Plugin?

Answer:
To dynamically provision Jenkins build agents inside Kubernetes.
