# Jenkins Logs

## What are Jenkins Logs?

Logs help administrators and DevOps engineers monitor Jenkins activities and troubleshoot issues.

Logs contain:

- Build Information
- Errors
- Warnings
- Plugin Activities
- System Events

## Jenkins Service Logs

View Jenkins logs:

```bash
sudo journalctl -u jenkins -f
```

## Jenkins Log Location

```bash
/var/log/jenkins/
```

Common Files:

```text
jenkins.log
```

## Build Console Logs

Dashboard
↓
Job
↓
Build
↓
Console Output

## Real-Time Scenario

A build suddenly fails.

First step:

Check Console Output and Jenkins Logs.

## Interview Question

Q: Where do you check Jenkins errors?

Answer:
Console Output, Jenkins Service Logs, and System Logs.
