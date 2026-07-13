# AWS 3-Tier Java Application Deployment using Terraform

## Project Overview

This project demonstrates the deployment of a Java web application on AWS using a secure and scalable 3-tier architecture. The infrastructure is organized using Terraform modules and follows AWS best practices for networking, security, scalability, and monitoring.

The project is intended to provide hands-on experience with designing production-style cloud infrastructure and deploying enterprise web applications.

---

## Architecture

The application is divided into three logical layers:

### Presentation Layer
- Application Load Balancer
- Nginx Web Server
- Public Subnets

### Application Layer
- Apache Tomcat
- Java Web Application
- Auto Scaling Group
- Private Subnets

### Database Layer
- Amazon RDS MySQL
- Private Database Subnets

---

## Technologies Used

- AWS
- Terraform
- EC2
- VPC
- Application Load Balancer
- Auto Scaling Group
- IAM
- Security Groups
- Amazon RDS MySQL
- CloudWatch
- Nginx
- Apache Tomcat
- Maven
- Git
- GitHub

---

## Project Structure

```
.
├── infrastructure
│   ├── main.tf
│   ├── variables.tf
│   └── modules
│       ├── vpc
│       ├── security
│       ├── alb
│       ├── asg
│       └── rds
│
└── Java-Login-App
    ├── pom.xml
    ├── src
    └── README.md
```

---

## Infrastructure Components

The infrastructure includes:

- Custom VPC
- Public and Private Subnets
- Internet Gateway
- Route Tables
- Security Groups
- Application Load Balancer
- Auto Scaling Group
- Amazon RDS
- IAM Roles

Terraform modules are used to keep the infrastructure reusable and easy to maintain.

---

## Application Deployment

The Java application is built using Maven.

Build command:

```bash
mvn clean package
```

After successful build, the application can be deployed on Apache Tomcat running on Amazon EC2 instances.

---

## Security

This project follows standard AWS security practices.

- Private database subnet
- Security Group based communication
- IAM Roles
- Least privilege access
- Network isolation
- Controlled inbound traffic

---

## Monitoring

Monitoring can be implemented using:

- Amazon CloudWatch
- CloudWatch Logs
- EC2 Metrics
- RDS Metrics

These services help monitor application health and infrastructure performance.

---

## Deployment Workflow

1. Configure AWS CLI
2. Initialize Terraform

```bash
terraform init
```

3. Review execution plan

```bash
terraform plan
```

4. Provision infrastructure

```bash
terraform apply
```

5. Build Java application

```bash
mvn clean package
```

6. Deploy application to Tomcat

7. Verify application through the Load Balancer endpoint

---

## Features

- Modular Terraform code
- High Availability architecture
- Auto Scaling support
- Load Balancing
- Secure networking
- Infrastructure as Code
- Production-oriented deployment
- Easy to extend

---

## Future Improvements

- Docker containerization
- Amazon EKS
- GitHub Actions CI/CD
- Jenkins Pipeline
- Prometheus & Grafana
- AWS WAF
- AWS Secrets Manager
- Route53
- SSL using ACM

---

## Learning Outcomes

Working on this project helped strengthen practical knowledge of:

- AWS Networking
- Terraform Modules
- EC2 Deployment
- RDS Configuration
- Load Balancing
- Infrastructure Automation
- Java Application Deployment
- Cloud Security Best Practices

---

## Author

**Rishika Patel**

DevOps Engineer

GitHub:
https://github.com/rishika-patel-1

LinkedIn:
https://linkedin.com/in/rishika-patel-233966268

---

## Disclaimer

This repository represents my hands-on implementation and learning of deploying a Java application using AWS services and Terraform. It is intended for educational and portfolio purposes.