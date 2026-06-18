# GitHub Integration

## Purpose

Integrate Jenkins with GitHub for automatic builds.

## Workflow

Developer Push
↓
GitHub
↓
Webhook
↓
Jenkins
↓
Build

## Add GitHub Credentials

Manage Jenkins
↓
Credentials
↓
Add Credentials

## Configure Repository

Example:

https://github.com/company/project.git

## Enable Webhook

GitHub
↓
Settings
↓
Webhooks
↓
Add Webhook

Payload URL:

http://JENKINS-IP:8080/github-webhook/

## Benefits

- Automatic Build Trigger
- Faster Feedback
- Continuous Integration

## Interview Questions

Q: What is a GitHub Webhook?

Answer:
A webhook automatically notifies Jenkins when code changes occur in GitHub.
