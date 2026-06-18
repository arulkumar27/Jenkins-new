# Building Docker Images

## What is a Docker Image?

A Docker Image is a packaged application containing:

- Application Code
- Libraries
- Dependencies
- Runtime Environment

## Sample Dockerfile

```dockerfile
FROM openjdk:17

COPY target/app.jar app.jar

ENTRYPOINT ["java","-jar","app.jar"]
```

## Build Docker Image

```bash
docker build -t myapp:v1 .
```

## Verify Image

```bash
docker images
```

## Jenkins Pipeline Example

```groovy
stage('Build Docker Image') {
    steps {
        sh 'docker build -t myapp:v1 .'
    }
}
```

## Real-Time Scenario

After successful build:

Jenkins automatically creates a Docker image for deployment.

## Interview Question

Q: What is docker build?

Answer:
The docker build command creates a Docker image from a Dockerfile.
