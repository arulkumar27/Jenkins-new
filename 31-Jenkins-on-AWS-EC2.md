# Jenkins on AWS EC2

## Why Run Jenkins on EC2?

Many organizations host Jenkins on AWS EC2 because:

- Easy Scalability
- High Availability
- Cloud-Based Infrastructure
- Cost Effective

## Architecture

Developer
↓
GitHub
↓
Jenkins (EC2)
↓
Docker
↓
Kubernetes / EC2

## Launch EC2

Recommended:

- Amazon Linux 2023
- t2.medium or higher
- Security Group:
  - 22 (SSH)
  - 8080 (Jenkins)

## Install Jenkins

```bash
sudo dnf update -y
sudo dnf install java-17-amazon-corretto -y
sudo wget -O /etc/yum.repos.d/jenkins.repo \
https://pkg.jenkins.io/redhat-stable/jenkins.repo
sudo rpm --import https://pkg.jenkins.io/redhat-stable/jenkins.io-2023.key
sudo dnf install jenkins -y
sudo systemctl enable jenkins
sudo systemctl start jenkins
```

## Access Jenkins

```text
http://PUBLIC-IP:8080
```

## Real-Time Scenario

A DevOps team hosts Jenkins on EC2 and manages deployments for hundreds of applications.

## Interview Question

Q: Why deploy Jenkins on EC2?

Answer:
EC2 provides a scalable and reliable cloud environment for Jenkins.
