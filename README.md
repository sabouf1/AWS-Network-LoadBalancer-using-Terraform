# AWS Network Load Balancer with Terraform

This repository contains the Terraform code required to deploy a Network Load Balancer in AWS that directs traffic to EC2 instances running Apache and Nginx. It's intended to be a hands-on lab to familiarize users with Terraform and AWS services.

## Lab Steps Overview

### Task 1: AWS Management Console Sign-In
- Navigate to the AWS Console.
- Sign in using the provided IAM user credentials.
- Set the AWS Region to US East (N. Virginia) `us-east-1`.

### Task 2: Setup Visual Studio Code
- Open Visual Studio Code.
- Open a new terminal by selecting `View -> Terminal`.
- Navigate to the Desktop with `cd Desktop`.
- Create a new directory `mkdir task_10125` and navigate into it `cd task_10125`.

### Task 3: Create a Variable File
- Inside the `task_10125` directory, create `variables.tf` and `terraform.tfvars` with global variables and their values.
- Run `code variables.tf` and `code terraform.tfvars` to open and edit these files in VS Code.

### Task 4: Launch an EC2 Instance
- Define the AWS provider and resources in `main.tf`.
- Create `main.tf` using `code main.tf` and input the Terraform code for launching an EC2 instance.

### Task 5: Create Network Load Balancer
- Extend `main.tf` to include the setup of a Network Load Balancer, target groups, and listeners.

### Task 6: Create an Output File
- Create `output.tf` with `code output.tf` to capture the ID and ARN of created resources.

### Task 7: Confirm Terraform Installation
- Check Terraform installation with `terraform version`.
- Install Terraform if not present, following the official guide.

### Task 8: Apply Terraform Configurations
- Initialize Terraform with `terraform init`.
- Plan deployment with `terraform plan`.
- Apply configurations with `terraform apply` and confirm with `yes`.

### Task 9: Check Resources in AWS Console
- Verify EC2 instance and Load Balancer creation in the AWS Console.

### Task 10: Install and Configure Nginx Services
- SSH into the EC2 instance and install Nginx.
- Configure Nginx to listen on port 8080 by editing the `nginx.conf`.

### Task 11: Testing Network Load Balancer
- Test traffic routing of the Network Load Balancer by accessing the provided DNS names.

### Task 12: Validation Test
- Perform a validation test by clicking the Validation button in the lab interface.

### Task 13: Delete AWS Resources
- Remove all resources with `terraform destroy` and confirm with `yes`.

## Setup Instructions

1. Clone the repository:
   ```bash
   git clone <repository-url>
