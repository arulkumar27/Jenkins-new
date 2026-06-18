# Deploy Applications to Kubernetes

## Deployment Process

Developer Push
↓
Jenkins Build
↓
Docker Image
↓
Kubernetes Deployment

## Deployment YAML

```yaml
apiVersion: apps/v1
kind: Deployment

metadata:
  name: myapp

spec:
  replicas: 2

  selector:
    matchLabels:
      app: myapp

  template:
    metadata:
      labels:
        app: myapp

    spec:
      containers:
      - name: myapp
        image: username/myapp:v1
```

## Deploy Command

```bash
kubectl apply -f deployment.yaml
```

## Jenkins Stage

```groovy
stage('Deploy') {
    steps {
        sh 'kubectl apply -f deployment.yaml'
    }
}
```

## Interview Question

Q: Which command deploys applications to Kubernetes?

Answer:
kubectl apply -f deployment.yaml
