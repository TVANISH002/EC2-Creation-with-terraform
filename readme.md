# 🚀 AWS Infrastructure Provisioning with Terraform

This project demonstrates a **production-style Infrastructure as Code (IaC) setup** using Terraform to provision and manage AWS resources. It follows best practices such as **remote state management, state locking, and modular infrastructure design**.

---

## 📌 Overview

The goal of this project is to provision a scalable and maintainable AWS infrastructure setup using Terraform, including:

* EC2 instance deployment
* Remote state management using S3
* State locking using DynamoDB
* Clean and reusable Terraform configuration

This setup mimics real-world DevOps workflows where infrastructure is version-controlled, automated, and reproducible.

---

## 🏗️ Architecture

* **EC2 Instance** → Compute resource
* **S3 Bucket** → Stores Terraform remote state
* **DynamoDB Table** → Prevents concurrent state updates (locking mechanism)

---

## 🛠️ Tech Stack

* **Terraform** (Infrastructure as Code)
* **AWS Services**

  * EC2
  * S3
  * DynamoDB
* **AWS CLI**

---

## ⚙️ Prerequisites

Ensure the following are installed and configured:

* Terraform (>= 1.x)
* AWS CLI configured with appropriate IAM permissions

Run:
aws configure
terraform -v

---

## 🔐 Security & Best Practices

* Remote state stored securely in S3
* State locking enabled using DynamoDB
* Sensitive values managed via variables (no hardcoding)
* `.gitignore` excludes `.tfstate` and sensitive files

---

## 🚀 Deployment Steps

Initialize Terraform:
terraform init

Validate configuration:
terraform validate

Review execution plan:
terraform plan

Apply infrastructure:
terraform apply

---

## 📊 Outputs

After successful deployment, Terraform provides:

* EC2 Public IP address
* Resource metadata

---

## 🧹 Teardown

To destroy all resources and avoid unnecessary costs:
terraform destroy

---

## 📈 Key DevOps Concepts Demonstrated

* Infrastructure as Code (IaC)
* Idempotent deployments
* Remote backend configuration
* State management and locking
* Environment reproducibility
* Version-controlled infrastructure

---


