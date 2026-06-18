# Pipeline Troubleshooting

## Common Pipeline Issues

### Syntax Errors

Example:

```groovy
pipeline {
agent any
stages {
```

Missing braces.

### Missing Tools

Example:

```bash
mvn: command not found
```

### Permission Problems

Deployment access denied.

### Agent Failures

Pipeline cannot execute.

## Debugging Steps

### Review Console Output

Most important step.

### Validate Jenkinsfile

Check syntax carefully.

### Verify Agent Availability

Ensure build node is online.

### Verify Credentials

Confirm credentials are valid.

## Real-Time Scenario

Pipeline fails during deployment.

Root Cause:

Expired AWS credentials.

## Interview Question

Q: How do you troubleshoot Jenkins pipelines?

Answer:
Check console logs, validate Jenkinsfile syntax, verify tools, agents, and credentials.
