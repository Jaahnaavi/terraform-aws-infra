# AWS Infrastructure Provisioning with Terraform

This project demonstrates Infrastructure as Code (IaC) using Terraform to provision and manage AWS infrastructure.

The infrastructure includes:

- AWS EC2 Instance
- AWS Security Group
- Automated Nginx Installation
- Public Web Server Deployment
- Infrastructure Lifecycle Management using Terraform

---

## Technologies Used

- Terraform
- AWS EC2
- AWS Security Groups
- Linux (Ubuntu)
- Nginx
- Git
- GitHub

---

## Architecture

Terraform
    ↓
AWS Provider
    ↓
Security Group
    ↓
EC2 Instance
    ↓
User Data Script
    ↓
Nginx Web Server

---

## Infrastructure Components

### Security Group

Allows:

- SSH (Port 22)
- HTTP (Port 80)

### EC2 Instance

- Ubuntu-based EC2 instance
- Provisioned using Terraform
- Configured automatically using user_data

### Nginx

Installed automatically during instance creation.

Custom landing page:

```html
<h1>Deployed with Terraform on AWS</h1>
```

---

## Terraform Commands

Initialize Terraform:

```bash
terraform init
```

Validate configuration:

```bash
terraform validate
```

Preview infrastructure changes:

```bash
terraform plan
```

Create infrastructure:

```bash
terraform apply
```

Destroy infrastructure:

```bash
terraform destroy
```

---

## Project Structure

```text
terraform-aws-infra/
├── main.tf
├── provider.tf
├── outputs.tf
├── README.md
└── .gitignore
```

---

## Skills Demonstrated

- Infrastructure as Code (IaC)
- AWS Cloud Provisioning
- Terraform Configuration
- Security Group Management
- Linux Server Automation
- Nginx Deployment
- Git Version Control

---

## Future Improvements

- Provision VPC and Subnets
- Create Auto Scaling Group
- Add Load Balancer
- Deploy Dockerized Applications
- Use Terraform Modules
