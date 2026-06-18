# GitHub Integration Issues

## Common Problems

### Invalid Credentials

GitHub authentication fails.

### Incorrect Repository URL

Repository cannot be accessed.

### Webhook Failure

Build not triggered.

### Network Issues

GitHub unreachable.

## Troubleshooting

### Verify Credentials

Manage Jenkins
↓
Credentials

### Test Repository Access

```bash
git clone REPOSITORY_URL
```

### Verify Webhook

GitHub
↓
Settings
↓
Webhooks

## Real-Time Scenario

Developer pushes code.

Build does not start.

Root Cause:

Webhook misconfigured.

## Interview Question

Q: Why are GitHub webhooks important?

Answer:
They automatically trigger Jenkins builds when code changes occur.
