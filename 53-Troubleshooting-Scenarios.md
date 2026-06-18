# Troubleshooting Scenarios

## Jenkins Not Starting

Check:

```bash
sudo systemctl status jenkins
```

Review:

```bash
sudo journalctl -xeu jenkins
```

---

## Docker Build Failure

Check:

```bash
docker images
```

Verify Docker Daemon:

```bash
systemctl status docker
```

---

## Maven Build Failure

Check:

```bash
mvn -version
```

Verify dependencies.

---

## Agent Offline

Check:

```bash
java -version
```

Verify connectivity and firewall rules.
