# Installing Docker in Jenkins

## Why Integrate Docker with Jenkins?

Docker helps package applications into containers.

Jenkins automates the Docker build and deployment process.

Benefits:

- Consistent Environments
- Faster Deployments
- Easy Scaling
- Platform Independence

## Install Docker

### Amazon Linux

```bash
sudo dnf install docker -y
```

### Start Docker

```bash
sudo systemctl enable docker
sudo systemctl start docker
```

### Verify Installation

```bash
docker --version
```

## Add Jenkins User to Docker Group

```bash
sudo usermod -aG docker jenkins
```

Restart Jenkins:

```bash
sudo systemctl restart jenkins
```

## Verify Access

```bash
docker ps
```

## Real-Time Scenario

Developer pushes code.

Jenkins:

- Builds Application
- Creates Docker Image
- Pushes Image to Registry

## Interview Question

Q: Why add Jenkins user to Docker group?

Answer:
To allow Jenkins jobs to execute Docker commands without root access.
