# Jenkins with IAM Roles

## What is an IAM Role?

IAM Role provides temporary AWS permissions.

Recommended over Access Keys.

## Traditional Method

Access Key
↓
Secret Key
↓
Stored in Jenkins

Risk:
- Credential Exposure

## Recommended Method

EC2
↓
IAM Role
↓
Temporary Permissions

## Benefits

- Better Security
- No Hardcoded Credentials
- Easier Management

## Real-Time Scenario

Jenkins uploads files to S3 using IAM Roles attached to EC2.

## Interview Question

Q: Why use IAM Roles instead of Access Keys?

Answer:
IAM Roles provide secure temporary credentials without storing secrets.
