# Scripted Pipeline

## What is Scripted Pipeline?

Scripted Pipeline uses Groovy scripting.

Provides more flexibility than Declarative Pipeline.

## Example

```groovy
node {

    stage('Build') {
        echo 'Building'
    }

    stage('Test') {
        echo 'Testing'
    }

    stage('Deploy') {
        echo 'Deploying'
    }

}
```

## Advantages

- More Flexible
- Supports Complex Logic
- Advanced Automation

## Disadvantages

- Harder to Read
- Difficult Maintenance

## Declarative vs Scripted

Declarative:
- Simple
- Structured
- Recommended

Scripted:
- Flexible
- Advanced
- Complex

## Real-Time Scenario

Large organizations use Scripted Pipelines for advanced deployment logic.

## Interview Question

Q: Difference between Declarative and Scripted Pipeline?

Answer:
Declarative Pipeline uses structured syntax while Scripted Pipeline uses Groovy scripting for greater flexibility.
