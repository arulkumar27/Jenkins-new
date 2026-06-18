# Pushing Images to Docker Hub

## What is Docker Hub?

Docker Hub is a cloud-based container image registry.

Used to store and share Docker images.

## Login

```bash
docker login
```

## Tag Image

```bash
docker tag myapp:v1 username/myapp:v1
```

## Push Image

```bash
docker push username/myapp:v1
```

## Jenkins Pipeline

```groovy
stage('Push Image') {
    steps {
        sh 'docker push username/myapp:v1'
    }
}
```

## Real-Time Workflow

Build
↓
Docker Image
↓
Docker Hub
↓
Kubernetes Deployment

## Benefits

- Central Repository
- Easy Distribution
- Version Management

## Interview Question

Q: Why push images to Docker Hub?

Answer:
To store Docker images centrally and make them available for deployment.
