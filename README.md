# ☁️ Azure VM Infrastructure using Terraform - Implicit Dependencies

<p align="center">
  <img src="https://img.shields.io/badge/Cloud-Azure-blue?logo=microsoftazure" />
  <img src="https://img.shields.io/badge/IaC-Terraform-623CE4?logo=terraform" />
  <img src="https://img.shields.io/badge/CI/CD-GitHub_Actions-black?logo=githubactions" />
  <img src="https://img.shields.io/badge/Auth-OIDC-green" />
  <img src="https://img.shields.io/badge/OS-Ubuntu-orange?logo=ubuntu" />
</p>

A lightweight Azure infrastructure project built using Terraform to demonstrate how **Implicit Dependencies** work in real-world Infrastructure as Code deployments.

This repository is also integrated with **GitHub Actions CI/CD automation**, allowing Azure infrastructure to be provisioned automatically using workflow pipelines and OIDC-based authentication.

---

# 🚀 Main Objective

This repository is mainly used for:

✅ Understanding Terraform Implicit Dependencies  
✅ Lightweight Azure VM Deployments  
✅ Infrastructure Testing & Validation  
✅ GitHub Actions CI/CD Practice  
✅ Azure + GitHub Integration  
✅ OIDC Authentication Practice  
✅ Fast Infrastructure Provisioning  

---

# 🔗 Terraform Implicit Dependencies

Terraform automatically understands resource relationships using resource references.

Example:

```hcl
subnet_id = azurerm_subnet.snet.id
```

Here Terraform automatically understands:

- NIC depends on Subnet
- VM depends on NIC
- Subnet depends on VNET

without manually using:

```hcl
depends_on
```

---

# ⚙️ Dependency Flow

```text
Resource Group
       ↓
Virtual Network
       ↓
Subnet
       ↓
Public IP
       ↓
Network Interface
       ↓
Linux Virtual Machine
```

---

# 🚀 GitHub Actions Automation

This project is also automated using **GitHub Actions** and Azure authentication workflows.

The repository contains multiple workflow YAML files used for:

- Azure authentication testing
- OIDC integration
- Terraform automation
- Infrastructure deployment pipelines

---

# 🔐 OIDC Authentication Workflow

One workflow file demonstrates how GitHub Actions can authenticate securely with Azure using OIDC (OpenID Connect).

### ✨ Benefits

✅ No hardcoded credentials  
✅ Secure Azure login  
✅ Token-based authentication  
✅ Recommended modern authentication method  

### ⚙️ Workflow

```text
GitHub Actions
       ↓
OIDC Authentication
       ↓
Azure Login
       ↓
Secure Cloud Access
```

---

# ☁️ Full Infrastructure Deployment Workflow

Another workflow file demonstrates complete Azure infrastructure automation.

### 🔥 Workflow Process

```text
Push Code to GitHub
       ↓
GitHub Actions Triggered
       ↓
Azure Authentication
       ↓
Terraform Init & Plan
       ↓
Terraform Apply
       ↓
Azure Infrastructure Provisioned
```

This workflow automatically provisions Azure resources directly from GitHub Actions pipelines.

---

# 🔄 GitHub Actions + Azure Integration

This repository highlights how GitHub Actions can be connected with Azure for Infrastructure as Code automation.

### Integrated Technologies

- GitHub Actions
- Azure Login Action
- Terraform
- OIDC Authentication
- Azure Resource Provisioning

---

# ✨ Features

✅ Terraform Implicit Dependency Practice  
✅ Lightweight Azure Infrastructure  
✅ Fast VM Deployment  
✅ GitHub Actions Automation  
✅ Azure OIDC Authentication  
✅ CI/CD Infrastructure Provisioning  
✅ Infrastructure Testing Environment  
✅ Beginner Friendly Terraform Setup  

---

# 🧪 Common Use Cases

- Terraform learning
- Implicit dependency understanding
- GitHub Actions testing
- Azure OIDC practice
- CI/CD experimentation
- Lightweight VM deployments
- Infrastructure automation testing

---

# 📂 Project Structure

```bash
azure-implicit-dependencies/
│
├── .github/workflows/
│   ├── azure-login.yml
│   └── terraform-deploy.yml
│
├── main.tf
├── provider.tf
├── variables.tf
├── outputs.tf
└── README.md
```

---

# 📦 Technologies Used

- ☁️ Microsoft Azure
- 🏗️ Terraform
- ⚙️ GitHub Actions
- 🔐 OIDC Authentication
- 🐧 Ubuntu Linux
- 🚀 Infrastructure as Code

---

# 📸 Preview

<p align="center">
  <img src="https://cdn-icons-png.flaticon.com/512/873/873107.png" width="120" />
  <img src="https://cdn-icons-png.flaticon.com/512/5968/5968705.png" width="120" />
  <img src="https://cdn-icons-png.flaticon.com/512/919/919853.png" width="120" />
  <img src="https://cdn-icons-png.flaticon.com/512/5968/5968875.png" width="120" />
</p>

---

# 🎯 Learning Outcome

By using this repository, you can understand:

✅ Terraform implicit dependencies  
✅ Azure infrastructure provisioning  
✅ GitHub Actions CI/CD  
✅ OIDC authentication with Azure  
✅ Infrastructure automation pipelines  
✅ Resource dependency flow  

---

# 👨‍💻 Author

### Abhishek Patil

Azure | Terraform | GitHub Actions | DevOps Enthusiast 🚀

---

# ⭐ Support

If you found this repository useful, consider giving it a ⭐ on GitHub.
