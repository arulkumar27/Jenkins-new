# Multi-Stage Docker Builds

## Problem

Normal Docker images are large.

Large images:

- Slow Downloads
- More Storage Usage
- Longer Deployments

## Solution

Multi-Stage Builds.

## Example

```dockerfile
FROM maven:3.9 AS build

WORKDIR /app

COPY . .

RUN mvn clean package

FROM openjdk:17

COPY --from=build /app/target/app.jar app.jar

ENTRYPOINT ["java","-jar","app.jar"]
```

## Benefits

- Smaller Images
- Faster Deployments
- Improved Security

## Real-Time Scenario

Production applications use multi-stage builds to reduce image size.

## Interview Question

Q: Why use Multi-Stage Docker Builds?

Answer:
To reduce image size by excluding unnecessary build dependencies.
