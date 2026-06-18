# GitHub Webhooks

## What is a Webhook?

A webhook sends notifications from GitHub to Jenkins when code changes occur.

## Workflow

Developer Pushes Code
↓
GitHub Webhook
↓
Jenkins Triggered
↓
Build Starts

## Webhook URL

```text
http://JENKINS-IP:8080/github-webhook/
```

## Benefits

- Automatic Builds
- Faster Feedback
- No Manual Triggering

## Real-Time Scenario

Developer commits code.

Within seconds Jenkins starts the build automatically.

## Interview Question

Q: Why use Webhooks?

Answer:
Webhooks automatically trigger Jenkins jobs whenever code changes occur in Git repositories.
