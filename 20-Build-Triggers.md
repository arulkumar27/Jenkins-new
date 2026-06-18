# Build Triggers

## What are Build Triggers?

Build Triggers define when Jenkins should start a job.

## Common Triggers

### Manual Trigger

User clicks:

```text
Build Now
```

### GitHub Webhook Trigger

Code Push
↓
Build Starts

### Poll SCM

Jenkins periodically checks Git repository.

Example:

```text
H/5 * * * *
```

Checks every 5 minutes.

### Scheduled Build

Run builds at fixed times.

Example:

```text
0 2 * * *
```

Runs daily at 2 AM.

## Real-Time Scenario

Nightly Testing Pipeline

Every night:

- Build Application
- Run Tests
- Generate Reports

Automatically triggered at 2 AM.

## Interview Question

Q: What are Jenkins Build Triggers?

Answer:
Build Triggers are mechanisms that automatically or manually start Jenkins jobs based on predefined conditions.
