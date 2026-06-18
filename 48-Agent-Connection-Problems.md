# Agent Connection Problems

## Common Issues

### Network Connectivity

Agent cannot reach Jenkins.

### Firewall Blocks

Required ports closed.

### Java Not Installed

Agent requires Java.

### Credential Problems

SSH authentication failure.

## Troubleshooting

### Verify Connectivity

```bash
ping AGENT-IP
```

### Verify Java

```bash
java -version
```

### Check Agent Logs

Review connection errors.

## Real-Time Scenario

Build stuck in queue.

Reason:

Agent disconnected.

## Interview Question

Q: Why do Jenkins agents go offline?

Answer:
Network issues, authentication failures, firewall restrictions, or Java problems.
