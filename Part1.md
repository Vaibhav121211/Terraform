# 🌍 Terraform Notes – Part 1  

---

## 📌 Introduction

Terraform is an open-source **Infrastructure as Code (IaC)** tool developed by **HashiCorp**, used to define and provision infrastructure using a high-level configuration language known as **HCL (HashiCorp Configuration Language)**.

---

## 🎯 Why Use Terraform?

### 🔧 Real-World Challenge:
Setting up secure cloud environments manually is:
- Time-consuming
- Error-prone
- Non-reusable

Example: AWS Hardening required 100–250+ pages of steps and took 2–3 days per account.

### ✅ Terraform Solution:
- Create **reusable code** that automates the deployment of identical infrastructure across accounts.
- Define infrastructure as code once, reuse it many times.
- Supports **multi-cloud and on-premises providers**.

---

## 🦸 Benefits of Terraform

- Provider-agnostic: Works with AWS, Azure, GCP, VMware, GitHub, etc.
- Supports reusable, version-controlled, declarative code.
- Manages entire infrastructure lifecycle (create, update, delete).

---

## 📚 About the Course

- Certification-specific content aligned with **Terraform Associate 2025** exam.
- Starts from **scratch** and gradually moves to **advanced** concepts.
- Uses **AWS** as the primary platform for demonstrations.

---

## 🧪 What Is Infrastructure as Code (IaC)?

IaC means managing infrastructure through **code** instead of manual configuration.

### Two Approaches:
1. **Manual:** Using cloud provider GUI/CLI.
2. **Automated (IaC):** Using tools like Terraform, Ansible, CloudFormation.

---

## ⚙️ Use Case Example – Automating Backups

**Manual Process:**  
Daily at 10 PM, take a DB backup and upload it to S3.

**Automated with IaC:**  
Use Terraform to define resources and schedule the task.

---

## 🚀 Benefits of IaC

- Faster provisioning  
- Reduced human error  
- Version control  
- Better collaboration  

---

## 🛠 Tools for IaC

| Category                    | Tools                                   |
|----------------------------|------------------------------------------|
| Infrastructure Orchestration | Terraform, CloudFormation, Heat          |
| Configuration Management     | Ansible, Chef, Puppet, SaltStack         |

### Key Difference:
- **Terraform** creates resources (servers, DBs, networks).
- **Ansible** manages configurations (e.g., install antivirus).

---

## 🤔 Choosing the Right IaC Tool

Ask yourself:
1. Are you locked into a single cloud vendor (like AWS)?
2. Will you use a hybrid/multi-cloud setup?
3. Do you need a GUI for automatic code generation?
4. What kind of support or documentation is available?

---

## 🧪 Sample Organizational Use Cases

### Org 1 – AWS-Only
- Wants GUI support.
- Needs vendor support.
- Committed to AWS for 25 years.

👉 **Best Tool:** CloudFormation or Terraform with commercial support.

### Org 2 – Hybrid (AWS + VMware + Azure + GCP)
- Needs cross-platform support.

👉 **Best Tool:** Terraform

---

## 🧰 Installation of Terraform

### 🔽 Simple Process:
- Download the **Terraform binary** from [terraform.io](https://www.terraform.io).
- Move it to your system's path:

```bash
sudo mv terraform /usr/local/bin/
