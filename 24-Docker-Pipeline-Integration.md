# Docker Pipeline Integration

## CI/CD Workflow

Developer Push
↓
GitHub
↓
Jenkins
↓
Build
↓
Docker Build
↓
Docker Push
↓
Deploy

## Sample Pipeline

```groovy
pipeline {

    agent any

    stages {

        stage('Build') {
            steps {
                sh 'mvn clean package'
            }
        }

        stage('Docker Build') {
            steps {
                sh 'docker build -t myapp:v1 .'
            }
        }

        stage('Push Image') {
            steps {
                sh 'docker push username/myapp:v1'
            }
        }
    }
}
```

## Benefits

- Full Automation
- Faster Releases
- Reduced Human Errors

## Real-Time Scenario

Every code commit automatically generates a Docker image.

## Interview Question

Q: Why integrate Docker with Jenkins?

Answer:
To automate container image creation and deployment in CI/CD pipelines.
