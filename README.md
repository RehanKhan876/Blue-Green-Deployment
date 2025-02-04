Blue-Green CI/CD Deployment with Infrastructure Automation and Kubernetes Management

Project Description: A Blue-Green CI/CD Deployment Pipeline integrated with Infrastructure Automation and Kubernetes Management on Amazon EKS!

This project combines Terraform, Kubernetes, and modern CI/CD practices to streamline deployments, ensure seamless environment switching, and enhance security.

Infrastructure Deployment

Using Terraform, I automated:

Creating a VPC with subnets, internet gateways, and route tables.

* Designing security groups for EKS clusters and worker nodes with IAM roles for permissions

•Deploying an Amazon EKS cluste with worker nodes to manage Kubernetes

workloads.

This setup ensures fast, repeatable, and reliable infrastructure provisioning.

Pipeline Configuration

Built a robust CI/CD pipeline with:

* Maven3, Docker, Trivy and SonarQube for complete lifecycle automation.

* Environment variables like DEPLOY ENV DOCKER TAG. and WITCH TRAFFIC for flexible deployments.

Pipeline Stages

The pipeline automates key steps:

1. Git Checkout: Clones the GitHub repository.

2. Compile: Builds the project using Maven.

3. Tests: Executes unit tests.

4. Trivy FS Scan: Detects vulnerabilities in the filesystem.

5. SonarQube Analysis: Ensures code quality through quality gates.

6. Build: Packages the application into a deployable artifact.

7. Publish Artifacts to Nexus: Manages artifact versions in Nexus.

8. Docker Build & Push: Builds and pushes images to Docker Hub.

9. Trivy Image Scan: Scans Docker images for vulnerabilities.

Deployment Stages

MySQL Deployment. Configures and deploys MySQL on Kubernetes. Application Deployment: Deploys backend and frontend services.

Blue-Green Deployment: Dynamically switches between blue and green environments for zero-downtime rollouts.

Traffic Switching: Redirects traffic seamlessly using Kubernetes service patches.

* Verification: Validates health and stability post-deployment.
