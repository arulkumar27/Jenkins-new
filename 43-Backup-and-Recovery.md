# Backup and Recovery

## Why Backup Jenkins?

Jenkins stores:

- Jobs
- Pipelines
- Credentials
- Plugins
- Build History

Without backups, recovery becomes difficult.

## Jenkins Home Directory

```bash
/var/lib/jenkins
```

## Backup Command

```bash
sudo tar -czvf jenkins-backup.tar.gz /var/lib/jenkins
```

## Restore Command

```bash
sudo tar -xzvf jenkins-backup.tar.gz -C /
```

## Backup Strategy

Daily:
- Jenkins Home

Weekly:
- Full Backup

Monthly:
- Disaster Recovery Test

## Real-Time Scenario

EC2 instance crashes.

Restore backup to a new Jenkins server.

## Interview Question

Q: What is the most important Jenkins directory?

Answer:
/var/lib/jenkins because it contains all Jenkins data.
