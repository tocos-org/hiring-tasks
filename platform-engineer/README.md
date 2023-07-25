# Take Home Task: Platform Engineering

## Objective
Create a simplified CI/CD pipeline for a micro-service, leveraging Infrastructure as Code (IaC) principles. This task should reflect your ability to design scalable, maintainable, and secure systems.

## Background
Imagine we have a micro-service that returns the current balance of Tocos for a user. We need to be able to simulate deploying this service on AWS using LocalStack and have a basic monitoring setup.

## Requirements: 

1. **Micro-service Development:**
    - Using any of the mentioned languages (TypeScript, Java, Rust, Python), create a basic REST API that returns a fixed value for Tocos. For simplicity, the service can return a static JSON response with the current value of Tocos per user.

2. **Infrastructure Setup:**
    - Use Terraform to set up a simulated AWS infrastructure to host this service using LocalStack. This should include a mock of an EC2 instance or a Fargate task (whichever you're more comfortable with) and necessary networking components (like VPC, subnets, etc.).

3. **Containerization:**
    - Containerize the micro-service using Docker. The Dockerfile should be optimized for a small image size and should follow best practices.

4. **CI/CD Setup:**
    - Set up a basic CI/CD pipeline using Github Actions. The pipeline should:
        - Build the micro-service.
        - Create a Docker image.
        - Push the Docker image to a container registry (e.g., Docker Hub).
        - Deploy the micro-service to the simulated infrastructure on LocalStack using Terraform.

5. **Monitoring:**
    - Simulate a basic monitoring setup using mock data for:
        - CPU usage.
        - Memory usage.
        - Number of requests.
    - Create a basic dashboard using Grafana to visualize this data.

## Deliverables:
- Source code for the micro-service.
- Dockerfile.
- Terraform scripts.
- CI/CD pipeline configuration files.
- Monitoring setup scripts/configuration.
- A README that details:
    - The design choices made.
    - Instructions on how to run and deploy the service using LocalStack.
    - Any assumptions made.
    
## Evaluation Criteria:
- Clarity and maintainability of the code.
- Simulated infrastructure setup and usage of Infrastructure as Code principles.
- Containerization best practices.
- Efficiency and completeness of the CI/CD setup.
- Simulated monitoring and alerting setup.
- Documentation clarity and completeness.

## Note:
This task should be developed and tested locally using LocalStack. Be sure your code is written in a way that it could easily be migrated to a real AWS environment with minimal changes. 

Please push your solution to a github repository and send us the link to the repository or alternatively use git bundle to bundle up your submission, place the resulting file on a file sharing service and share the link to the file.

This task is designed to be completed in approximately two hours. If you find yourself spending significantly more time, try to simplify your approach and document any assumptions or shortcuts you have taken in the README file.

Good luck, and we're excited to see your approach to this challenge!
