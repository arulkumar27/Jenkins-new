# Deploy Applications to EC2

## Goal

Deploy applications automatically from Jenkins to EC2.

## Workflow

Developer Push
↓
GitHub
↓
Jenkins Build
↓
EC2 Deployment

## Configure SSH Access

Generate Key:

```bash
ssh-keygen
```

Copy Public Key:

```bash
ssh-copy-id ec2-user@SERVER-IP
```

## Jenkins Deployment Stage

```groovy
stage('Deploy') {

    steps {

        sh '''
        ssh ec2-user@SERVER-IP "
        docker pull username/myapp:v1
        docker stop myapp || true
        docker rm myapp || true
        docker run -d --name myapp -p 80:8080 username/myapp:v1
        "
        '''
    }
}
```

## Benefits

- Automated Deployment
- Faster Releases
- Reduced Human Errors

## Interview Question

Q: How does Jenkins deploy to EC2?

Answer:
Using SSH connections and deployment scripts executed from Jenkins pipelines.
