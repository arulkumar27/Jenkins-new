# Helm Integration

## What is Helm?

Helm is the package manager for Kubernetes.

It simplifies application deployment.

## Benefits

- Reusable Templates
- Easy Upgrades
- Easy Rollbacks

## Install Application

```bash
helm install myapp mychart
```

## Upgrade Application

```bash
helm upgrade myapp mychart
```

## Rollback Application

```bash
helm rollback myapp 1
```

## Jenkins Pipeline Example

```groovy
stage('Helm Deploy') {
    steps {
        sh 'helm upgrade --install myapp mychart'
    }
}
```

## Interview Question

Q: Why use Helm?

Answer:
Helm simplifies Kubernetes application deployment and management.
