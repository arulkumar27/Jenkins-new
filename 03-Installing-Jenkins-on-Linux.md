# Installing Jenkins on Linux

## Prerequisites

- Linux Server
- Root Access
- Internet Connection
- Java Installed

## Update Packages

```bash
sudo dnf update -y
```

## Install Java

```bash
sudo dnf install java-17-amazon-corretto -y
```

## Verify Java

```bash
java -version
```

## Add Jenkins Repository

```bash
sudo wget -O /etc/yum.repos.d/jenkins.repo \
https://pkg.jenkins.io/redhat-stable/jenkins.repo
```

## Import Jenkins Key

```bash
sudo rpm --import https://pkg.jenkins.io/redhat-stable/jenkins.io-2023.key
```

## Install Jenkins

```bash
sudo dnf install jenkins -y
```

## Start Jenkins

```bash
sudo systemctl enable jenkins
sudo systemctl start jenkins
```

## Verify Status

```bash
sudo systemctl status jenkins
```

## Open Jenkins

http://SERVER-IP:8080

## Interview Questions

Q: Which port does Jenkins use?

Answer:
8080 by default.
