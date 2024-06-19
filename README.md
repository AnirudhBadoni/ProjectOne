# Project Title: Infrastructure Deployment using IaC and CI/CD Pipeline Implementation

## Overview
This project is a proof of concept commissioned by a client to demonstrate the ability to build a scalable and secure infrastructure using Infrastructure as Code (IaC) practices on AWS/Azure and establish a robust DevOps pipeline for building and deploying a Java application. The project is divided into three main parts: creating a base Amazon Machine Image (AMI) using Packer, containerizing a Java application and implementing a CI/CD pipeline, and deploying the infrastructure using Terraform.

## Project Breakdown:

The project is divided into three parts
|[Part 1](https://github.com/AnirudhBadoni/Packer.git)|[Part 2](https://github.com/AnirudhBadoni/Petclinic.git)|[Part 3](https://github.com/AnirudhBadoni/AwsInfra.git)|
|---|---|---|

## Part 1: Creation of a Base AMI using Packer

<p align="center">
  <img src="./one.png">
</p>

**Objective:** Build a base AMI with the required software pre-installed.
**Tools:** Packer, AWS/Azure
**Software to be Installed:**
1. CloudWatch Agent
2. AWS SSM Agent
3. Docker
4. Git Client
**Provisioning:** Use shell script for beginners and Ansible for more experienced participants.
**CI Tool:** Any CI tool of choice (e.g., Jenkins, GitHub Actions) to build the Packer pipeline.

## Part 2: Containerizing a Java Application and Implementing a CI/CD Pipeline

<p align="center">
  <img src="./two.png">
</p>

**Objective:** Build and containerize a Java application, scan the code, and push the container to a repository.<br>
**Tools:** GitLab, Azure DevOps, Jenkins, GitHub Actions, JFrog Artifactory, SonarCloud<br>
**Steps:**
1. Containerize the application using Docker.
2. Implement a CI/CD pipeline to build the application and produce a container image.
3. Scan the code and Docker files using SonarCloud.
4. Push the container image to JFrog Artifactory.

## Part 3: Deploying Infrastructure Using Terraform

<p align="center">
  <img src="./Three.png">
</p>
</details>

**Objective:** Deploy a secure, scalable infrastructure.
**Tools:** Terraform, AWS/Azure
**Infrastructure Components:**
1. VPC with Public, Private, and Secure subnets
2. Load Balancer in Public Subnet
3. Auto Scaling Group in Private Subnet
4. RDS Cluster in Secure Subnet
**Best Practices:**
1. Store state in S3/Azure Blob with cross-region replication and encryption.
2. Enable state locking using DynamoDB.
3. Use the GitOps approach for Terraform to apply on merge to the main branch.
