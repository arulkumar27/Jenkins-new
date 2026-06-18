# Upgrading Jenkins

## Why Upgrade Jenkins?

Benefits:

- Security Fixes
- New Features
- Bug Fixes
- Better Performance

## Check Current Version

Dashboard
↓
Manage Jenkins
↓
System Information

## Upgrade Steps

### Stop Jenkins

```bash
sudo systemctl stop jenkins
```

### Update Packages

```bash
sudo dnf update jenkins -y
```

### Start Jenkins

```bash
sudo systemctl start jenkins
```

### Verify

```bash
sudo systemctl status jenkins
```

## Best Practice

Take Backup Before Upgrade.

## Interview Question

Q: What should you do before upgrading Jenkins?

Answer:
Take a full backup of Jenkins Home Directory.
