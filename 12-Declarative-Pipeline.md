# Declarative Pipeline

## What is Declarative Pipeline?

Declarative Pipeline is a structured and easy-to-read pipeline syntax.

Recommended by Jenkins.

## Example

```groovy
pipeline {
    agent any

    stages {

        stage('Build') {
            steps {
                echo 'Build Stage'
            }
        }

        stage('Test') {
            steps {
                echo 'Test Stage'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploy Stage'
            }
        }
    }
}
```

## Main Components

### Agent

Defines execution environment.

```groovy
agent any
```

### Stage

Represents a phase.

```groovy
stage('Build')
```

### Steps

Commands executed inside stages.

```groovy
steps {
   echo 'Building'
}
```

## Advantages

- Easy to Read
- Easy to Maintain
- Better Structure

## Real-Time Scenario

Build → Test → Docker Build → Deploy

All stages defined inside Jenkinsfile.

## Interview Question

Q: Why use Declarative Pipeline?

Answer:
It provides a structured and readable syntax for CI/CD workflows.
