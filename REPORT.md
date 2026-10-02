# Lab 1 - DevOps Foundations & Continuous Integration

## Objective

To implement a basic DevOps workflow using Git, GitHub and Jenkins for version control, continuous integration and automated deployment.

## Tools Used

- Ubuntu Linux (WSL2)
- Git
- GitHub
- Jenkins
- Java 21
- Python
- Pytest

## Version Control Workflow

A local Git repository was initialized for the Python application.

Changes were staged and committed using Git. Feature branches were created for unit testing and documentation. These branches were later merged into the main branch.

The completed repository was pushed to GitHub.

## CI/CD Architecture

GitHub Repository
↓
Jenkins
↓
Build
↓
Test
↓
Deploy

## Build Stage

Jenkins creates a Python virtual environment and installs project dependencies.

## Test Stage

Pytest executes automated unit tests.

Expected result:

2 tests passed successfully.

## Deploy Stage

After successful testing, Jenkins creates a deployment directory and copies the application into it.

The deployed Python application is executed to verify successful deployment.

## Automation

Jenkins Poll SCM is configured to periodically check the GitHub repository.

When a new commit is detected, Jenkins automatically starts the CI/CD pipeline.

## Result

The Jenkins pipeline successfully performed:

1. Source code checkout
2. Build
3. Automated testing
4. Deployment

The complete CI/CD workflow executed successfully.

## Conclusion

The experiment demonstrated a basic DevOps CI/CD workflow using Git, GitHub and Jenkins. Version control, automated builds, testing and deployment were successfully integrated.
