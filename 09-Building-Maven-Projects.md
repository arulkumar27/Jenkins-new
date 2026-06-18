# Building Maven Projects

## What is Maven?

Maven is a build automation tool primarily used for Java applications.

## Install Maven

Manage Jenkins
↓
Global Tool Configuration
↓
Add Maven

## Build Command

```bash
mvn clean install
```

## Build Stages

Source Code
↓
Compile
↓
Test
↓
Package
↓
Artifact

## Generated Files

```text
application.jar
application.war
```

## Real-Time Scenario

Developer pushes Java code.

Jenkins:

- Downloads Source Code
- Compiles Code
- Runs Unit Tests
- Creates JAR File

## Interview Questions

Q: What does mvn clean install do?

Answer:
It cleans old builds, compiles source code, runs tests, and creates deployable artifacts.
