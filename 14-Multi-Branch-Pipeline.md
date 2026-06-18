# Multi-Branch Pipeline

## What is Multi-Branch Pipeline?

Automatically creates Jenkins pipelines for each Git branch.

Example:

```text
main
develop
feature-login
feature-payment
```

Each branch gets its own pipeline.

## Benefits

- Automatic Branch Detection
- Faster Development
- Better CI/CD

## Workflow

Developer Creates Branch
↓
Push Code
↓
Jenkins Detects Branch
↓
Pipeline Created Automatically

## Real-Time Example

E-Commerce Project

Branches:

- main
- dev
- feature-cart
- feature-payment

Jenkins builds each branch separately.

## Advantages

- Reduced Manual Work
- Better Collaboration
- Faster Testing

## Interview Question

Q: Why use Multi-Branch Pipeline?

Answer:
To automatically discover and build multiple Git branches without creating separate jobs manually.
