# Multi-Environment AWS Infrastructure using Terraform

---

## 🛠️ **Project Overview**  
This project demonstrates the creation of a **multi-environment AWS infrastructure** using **Terraform**, an Infrastructure as Code (IaC) tool. It provisions cloud resources for **Development (DEV)**, **Staging (STG)**, and **Production (PRD)** environments, following best practices for modularity and scalability.

---

## 🌟 **Features**

- Multi-environment setup: **DEV**, **STG**, and **PRD**.
- Automated resource provisioning on AWS.
- Modularized Terraform code for reusability and maintainability.
- Environment-specific configurations.
- Scalable production infrastructure.

---

## 🌍 **Infrastructure Details**

### Resources Provisioned:

| Environment | S3 Buckets | DynamoDB Tables | EC2 Instances |
|-------------|------------|-----------------|---------------|
| **DEV**     | 1          | 1               | 1             |
| **STG**     | 1          | 1               | 1             |
| **PRD**     | 2          | 1               | 3             |

---

## 🛡️ **How It Works**

### 1️⃣ **Setup Environment**
- Install Terraform.
- Configure AWS CLI with valid credentials.

### 2️⃣ **Clone Repository**
```bash
git clone https://github.com/biswas-12/Multi-Environment-AWS-Infrastructure-using-Terraform.git
cd terraform-for-devops
```

### 3️⃣ **Initialize Terraform**
Run the following command to initialize Terraform and download necessary providers:
```bash
terraform init
```

### 4️⃣ **Deploy Infrastructure**
Choose the desired environment (DEV, STG, or PRD), navigate to the respective folder, and deploy resources:
```bash
cd envs/dev   # Example: Switch to the DEV environment
terraform plan
terraform apply
```

### 5️⃣ **Verify Resources**
Check the AWS Management Console to ensure the infrastructure is provisioned as expected.

### 6️⃣ **Destroy Infrastructure**
To clean up resources:
```bash
terraform destroy
```
