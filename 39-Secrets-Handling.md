# Secrets Handling

## What are Secrets?

Sensitive information such as:

- Passwords
- API Keys
- Access Tokens
- SSH Keys

## Bad Practice

```groovy
sh 'aws configure set aws_secret_access_key ABC123'
```

Never hardcode secrets.

## Good Practice

```groovy
withCredentials([
string(credentialsId: 'aws-key',
variable: 'AWS_KEY')
]) {

sh 'echo Secret Loaded'
}
```

## Benefits

- Improved Security
- Compliance
- Reduced Risk

## Real-Time Scenario

Jenkins securely retrieves secrets during deployment.

## Interview Question

Q: Why avoid hardcoded secrets?

Answer:
Hardcoded secrets can be exposed through repositories and logs.
