# Node.js Demo App CI/CD

This project shows how to set up a basic CI/CD pipeline using GitHub Actions and Docker.

## Tools Used
- Node.js
- GitHub Actions
- Docker
- DockerHub

## CI/CD Steps
1. On every push to main, the pipeline runs.
2. It installs dependencies and runs tests.
3. Then it builds a Docker image.
4. The image is pushed to DockerHub automatically.
