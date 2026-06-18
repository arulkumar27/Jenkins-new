# Pipeline as Code

## What is Pipeline as Code?

Pipeline as Code means defining the entire CI/CD workflow using code instead of configuring jobs manually through the Jenkins UI.

The pipeline is stored in a file called:

```text
Jenkinsfile
```

## Why Use Pipeline as Code?

Traditional Approach:

- Manual Configuration
- Difficult to Track Changes
- No Version Control

Pipeline as Code:

- Stored in GitHub
- Version Controlled
- Easy Rollback
- Reusable

## Basic Jenkinsfile

```groovy
pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building Application'
            }
        }
    }
}
```

## Benefits

- Automation
- Version Control
- Reusability
- Scalability

## Real-Time Scenario

Developer pushes Jenkinsfile into GitHub.

Jenkins automatically reads instructions and executes the pipeline.

## Interview Question

Q: What is Pipeline as Code?

Answer:
Pipeline as Code is the practice of defining CI/CD workflows using code stored in version control systems.
