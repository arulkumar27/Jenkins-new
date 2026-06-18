# Jenkins Agent Nodes

## What are Agents?

Agents are worker machines that execute Jenkins jobs.

## Why Use Agents?

Large organizations have:

- Multiple Projects
- Multiple Teams
- Hundreds of Builds

Single Jenkins server cannot handle everything.

## Types of Agents

### Linux Agent

Build Linux applications.

### Windows Agent

Build .NET applications.

### Docker Agent

Build containerized applications.

## Architecture

Jenkins Controller
|
|---- Linux Agent
|
|---- Windows Agent
|
|---- Docker Agent

## Benefits

- Faster Builds
- Scalability
- Resource Optimization
- Better Performance

## Real-Time Scenario

Master receives build request.

Master assigns build to available agent.

Agent executes build and returns result.

## Interview Questions

Q: Difference between Controller and Agent?

Answer:

Controller:
Manages Jenkins.

Agent:
Executes build jobs.
