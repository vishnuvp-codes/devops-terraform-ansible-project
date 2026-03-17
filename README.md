
# 🚀 DevOps Automation Project: Terraform + Ansible + Docker

## 📌 Project Overview

This project demonstrates **DevOps automation using Terraform and Ansible**. The goal is to automate infrastructure setup and server configuration, then deploy a containerized web application using Docker.

The automation workflow provisions infrastructure with Terraform and configures the system with Ansible to install Docker and run an Nginx container.

---

## ⚙️ Technologies Used

* **Linux (Ubuntu)**
* **Terraform** – Infrastructure as Code (IaC)
* **Ansible** – Configuration Management
* **Docker** – Containerization platform
* **YAML** – Ansible playbook configuration
* **Git & GitHub** – Version control

---

## 🏗️ Project Architecture

```
Terraform
   ↓
Infrastructure Setup
   ↓
Ansible Automation
   ↓
Docker Installation
   ↓
Nginx Container Deployment
   ↓
Web Server Running
```

---

## 📁 Project Structure

```
devops-automation-project
│
├── terraform
│   └── main.tf
│
└── ansible
    ├── inventory
    └── install-docker.yml
```

---

## 🔧 Terraform Configuration

Terraform is used to initialize infrastructure and demonstrate **Infrastructure as Code (IaC)**.

### Terraform Commands

Initialize Terraform:

```
terraform init
```

Apply configuration:

```
terraform apply
```

This executes the Terraform configuration and prepares the infrastructure environment.

---

## 🔧 Ansible Configuration

Ansible is used to automate server configuration.

### Inventory File

```
[servers]
localhost ansible_connection=local
```

### Ansible Playbook

The playbook performs the following tasks:

* Updates system packages
* Installs Docker
* Starts Docker service
* Deploys an Nginx container

Run the playbook:

```
ansible-playbook -i inventory install-docker.yml
```

---

## 🐳 Docker Deployment

After automation runs successfully, Docker deploys the Nginx container.

Check running containers:

```
docker ps
```

You should see the **nginx-server container running**.

---

## 🌐 Application Access

Open a browser and access:

```
http://localhost:8080
```

You should see the **Nginx Welcome Page**, confirming the application is running successfully.

---

## 📊 Key Learning Outcomes

This project demonstrates:

* Infrastructure provisioning using **Terraform**
* Server configuration automation using **Ansible**
* Containerized application deployment with **Docker**
* DevOps automation workflow
* Infrastructure as Code (IaC)

---

## 🚀 Future Improvements

Potential enhancements include:

* Deploy infrastructure on **AWS using Terraform**
* Automate cloud server configuration with **Ansible**
* Deploy applications on **Kubernetes**
* Implement **CI/CD pipelines**
* Add **monitoring using Prometheus and Grafana**

---

## 👩‍💻 Author

**Vishnupriya**

DevOps Enthusiast | Linux | Docker | Terraform | Ansible 
