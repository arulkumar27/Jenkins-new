# Kubernetes CI/CD Pipeline

## End-to-End Workflow

Developer Push
↓
GitHub
↓
Jenkins Trigger
↓
Build
↓
Unit Testing
↓
Docker Build
↓
Push to Docker Hub
↓
Kubernetes Deployment
↓
Production

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

        stage('Docker Push') {
            steps {
                sh 'docker push username/myapp:v1'
            }
        }

        stage('Kubernetes Deploy') {
            steps {
                sh 'kubectl apply -f deployment.yaml'
            }
        }
    }
}
```

## Production Benefits

- Faster Releases
- Automated Deployments
- Improved Reliability
- Reduced Downtime

## Real-Time Scenario

Enterprise DevOps teams deploy applications multiple times daily using Jenkins + Docker + Kubernetes.

## Interview Question

Q: Explain a Jenkins Kubernetes CI/CD Pipeline.

Answer:
Jenkins builds the application, creates a Docker image, pushes it to a registry, and deploys it automatically to Kubernetes.
