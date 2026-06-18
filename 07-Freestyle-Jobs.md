# Freestyle Jobs

## What is a Freestyle Job?

Freestyle Job is the simplest Jenkins job type.

Used for:

- Running Scripts
- Building Applications
- Automation Tasks

## Create Job

New Item
↓
Freestyle Project

## Build Step Example

```bash
echo "Hello Jenkins"
```

## Maven Build Example

```bash
mvn clean install
```

## Real-Time Scenario

Developer pushes code.

Freestyle Job:

- Pulls Code
- Builds Application
- Generates Artifact

## Advantages

- Easy Setup
- Beginner Friendly

## Disadvantages

- Difficult to maintain for complex workflows

## Interview Questions

Q: What is a Freestyle Job?

Answer:
A Freestyle Job is a basic Jenkins project used for executing build and automation tasks.
