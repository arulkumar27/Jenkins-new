# Production Support Questions

## What will you do if Jenkins server is down?

Answer:

1. Verify Service Status
2. Check Logs
3. Restore from Backup
4. Escalate if required

---

## What if disk space reaches 100%?

Answer:

```bash
df -h
```

Remove old logs and artifacts.

---

## What if builds become slow?

Answer:

- Check CPU
- Check Memory
- Review Agent Utilization

---

## What if Jenkins credentials expire?

Answer:

Update credentials and rerun pipeline.
