# Build and Push Docker Image to AWS ECR with GitHub Actions

This project is designed to build a Docker image from a Dockerfile and push it to AWS Elastic Container Registry (ECR) as an image snapshot using GitHub Actions.

## Project Structure

The repository is organized into several key directories:

- **.github/workflows**: Contains the GitHub Actions workflow file (`build.yml`) that automates the deployment process.
- **docker**: Includes the Dockerfile and any other necessary files for building the Docker image.

## Key Components

- **Docker**: Used to build the Docker image from the Dockerfile. The image contains the application and its dependencies.
- **AWS ECR**: A fully managed Docker container registry that makes it easy to store, manage, and deploy Docker container images.
- **GitHub Actions**: Automates the process of building the Docker image and pushing it to AWS ECR. The workflow is triggered whenever changes are pushed to the `main` branch.

## Workflow

1. **Dockerfile**: The `docker` directory contains the Dockerfile, which defines the application's environment and dependencies.
2. **GitHub Actions**: The workflow file (`build.yml`) in the `.github/workflows` directory automates the process of building the Docker image and pushing it to AWS ECR. It uses the AWS credentials stored as GitHub Secrets to authenticate and push the image.

## Summary

This project provides a structured and automated approach to building and deploying Docker images to AWS ECR using GitHub Actions. By organizing the repository and automating the workflow, it ensures a scalable and maintainable deployment process.
