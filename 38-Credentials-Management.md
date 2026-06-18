# Credentials Management

## Why Credentials Management?

Jenkins interacts with:

- GitHub
- Docker Hub
- AWS
- Kubernetes

Credentials must be stored securely.

## Credential Types

### Username and Password

GitHub Authentication.

### Secret Text

API Tokens.

### SSH Keys

Server Access.

### Secret Files

Kubeconfig Files.

## Add Credentials

Manage Jenkins
↓
Credentials
↓
Add Credentials

## Best Practices

- Never Hardcode Passwords
- Rotate Secrets Regularly
- Use IAM Roles Where Possible

## Interview Question

Q: Where should credentials be stored?

Answer:
Inside Jenkins Credentials Store or external secret management systems.
