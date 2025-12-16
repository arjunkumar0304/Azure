# Azure



## 1. Core Azure Architectural Components

### 1.1 Regions, Availability Zones, Resource Groups

#### Azure Region

* A **geographical location** where Microsoft has one or more data centers.
* Examples: **Central India, East US, West Europe**.



#### Availability Zones (AZ)

* **Physically separate data centers** within the same region.
* Each zone has independent **power, cooling, and networking**.



#### Resource Group

* A **logical container** for Azure resources like VM, Storage, Database, Network.
* Used for **organization, access control, monitoring, and lifecycle management**.

**Real‑world example:**
Like a folder that contains all files related to one project.



### 1.2 Azure Resource Manager (ARM)

* ARM is the **management layer** of Azure.
* Used to **create, update, delete, and manage resources**.
* Supports **Infrastructure as Code** using ARM templates (JSON).

**Key features:**

* Role‑Based Access Control (RBAC)
* Tagging
* Consistent deployments


### 1.3 Azure Compute Options

#### Virtual Machines (VM)

* Provides a **virtual computer** in the cloud.
* Full control over **OS, software, and configuration**.

**Use case:** Running custom applications, legacy software.


#### Azure App Services

* **Platform as a Service (PaaS)** for hosting web apps and APIs.
* Azure manages OS, patching, and scaling.

**Benefit:** Developer focuses only on code.



#### Containers

* Lightweight application packaging.
* Ensures applications run consistently across environments.

**Tools:** Docker, Kubernetes.


#### Azure Functions

* **Serverless computing service**.
* Runs code only when triggered (event‑based).
* Pay only for execution time.

**Example triggers:** HTTP request, timer, file upload.

---

## 2. Cloud Concepts

### 2.1 Cloud Service Models

#### IaaS (Infrastructure as a Service)

* User manages: OS, runtime, application.
* Azure manages: hardware, networking.

**Example:** Azure Virtual Machines.


---

#### PaaS (Platform as a Service)

* User manages: application and data.
* Azure manages: OS, runtime, infrastructure.

**Examples:** Azure App Services, Azure SQL Database.



#### SaaS (Software as a Service)

* Azure manages everything.
* Ready‑to‑use software over the internet.

**Examples:** Microsoft 365, Dynamics 365.


---

### 2.2 Cloud Deployment Models

* **Public Cloud:** Shared infrastructure (Azure, AWS).
* **Private Cloud:** Dedicated to a single organization.
* **Hybrid Cloud:** Combination of public and private cloud.



### 2.3 CapEx vs OpEx

#### CapEx (Capital Expenditure)

* High upfront investment.
* Traditional data centers.

#### OpEx (Operational Expenditure)

* Pay‑as‑you‑go model.
* No upfront hardware cost.


---

## 3. Azure Compute Services

### 3.1 Virtual Machines (VMs)

#### VM Sizing

* Based on CPU, RAM, and disk.
* Choose size based on workload.

---

#### VM Pricing

* Charged based on VM size and running time.
* Stopping a VM reduces cost.

---

#### VM Scaling

* **Vertical Scaling:** Increase CPU/RAM.
* **Horizontal Scaling:** Add more VMs.


---

#### VM Deployment & Management

* Azure Portal
* ARM Templates
* Azure CLI
* PowerShell

---

### 3.2 Azure App Services

* Fully managed PaaS service.
* Built‑in scaling and high availability.
* Minimal maintenance.

---

### 3.3 Azure Functions

* Serverless and event‑driven.
* Cost‑effective for short‑running tasks.

---

### 3.4 Azure Kubernetes Service (AKS)

* Managed Kubernetes service.
* Used for container orchestration and microservices.
* Supports auto‑scaling.

---

### 3.5 Cloud Service Models – Summary

| Model | Control Level | Example         |
| ----- | ------------- | --------------- |
| IaaS  | High          | Virtual Machine |
| PaaS  | Medium        | App Service     |
| SaaS  | Low           | Microsoft 365   |


# Azure Core Services – README

This document explains **core Azure services** in a simple and structured way. It is designed for **freshers**, **interview preparation**, and **basic project documentation**.

---

## 3. Azure Compute Services

Azure Compute Services provide **processing power** to run applications, services, and workloads in the cloud.

---

### 3.1 Virtual Machines (VMs)

**What it is:**
Azure Virtual Machines are **virtual servers** in the cloud that work like physical computers.

**Why it is used:**

* Full control over OS (Windows/Linux)
* Run legacy applications
* Custom software installation

**Example:**

* Hosting a Java or Python application
* Running a database or testing environment

---

#### 3.1.1 VM Sizing, Pricing, and Scaling

**VM Sizing:**
Choosing VM based on **CPU, RAM, and storage** requirements.

**Pricing:**

* Pay only for what you use
* Cost depends on VM size, OS, and usage hours

**Scaling:**

* **Vertical scaling:** Increase/decrease VM size
* **Horizontal scaling:** Add/remove VMs using Scale Sets

**Example:**

* Increase VM size during peak traffic

---

#### 3.1.2 VM Deployment and Management

**Deployment:**

* Create VMs using Azure Portal, CLI, ARM templates

**Management:**

* Monitoring with Azure Monitor
* Patching and updates
* Backup and recovery

---

### 3.2 Azure App Services

**What it is:**
A **Platform as a Service (PaaS)** for hosting web applications and APIs.

**Why it is used:**

* No server management
* Auto-scaling
* Built-in security

**Example:**

* Hosting a web application or REST API

---

### 3.3 Azure Functions

**What it is:**
A **serverless compute service** that runs code based on events.

**Why it is used:**

* Pay per execution
* Event-driven
* No infrastructure management

**Example:**

* Trigger function when a file is uploaded to Blob Storage

---

### 3.4 Azure Kubernetes Service (AKS)

**What it is:**
A managed service to run **containerized applications** using Kubernetes.

**Why it is used:**

* Manages containers
* High scalability
* Microservices architecture

**Example:**

* Deploying Docker-based applications

---

### 3.5 Cloud Service Models

* **IaaS (Infrastructure as a Service):** VMs, Networking
* **PaaS (Platform as a Service):** App Services, Azure SQL
* **SaaS (Software as a Service):** Microsoft 365

**Example:**

* VM → IaaS
* App Service → PaaS
* Outlook → SaaS

---

## 4. Azure Storage Services

Azure Storage provides **secure and scalable storage** for data.

---

### 4.1 Blob Storage

**What it is:**
Used to store **unstructured data** such as images, videos, documents, and backups.

**Example:**

* Store application images or logs

---

### 4.2 Storage Tiers and Replication

**Storage Tiers:**

* Hot – Frequently accessed data
* Cool – Infrequently accessed data
* Archive – Rarely accessed data

**Replication Types:**

* LRS – Local redundancy
* ZRS – Zone redundancy
* GRS – Geo redundancy

**Purpose:**
Ensures data availability and disaster recovery.

---

### 4.3 Access Control and Shared Access Signatures (SAS)

**Access Control:**
Uses Azure AD and RBAC to control access.

**SAS:**
Provides temporary and limited access to storage resources.

**Example:**

* Share a file link valid for 1 day

---

## 5. Azure Key Vault, Azure Functions, Azure Logic Apps

### Azure Key Vault

Stores **secrets, passwords, keys, and certificates** securely.

**Example:**

* Store database credentials

---

### Azure Functions

Runs event-based code without managing servers.

---

### Azure Logic Apps

Used to create **automated workflows** with minimal code.

**Example:**

* Send email when a file is uploaded

---

## 6. Azure Data Services

Azure Data Services help store, process, and move data.

---

### 6.1 Azure Data Factory (ADF)

A cloud-based **data integration service**.

---

#### 6.1.1 Data Ingestion and Transformation

* Ingestion: Collect data from different sources
* Transformation: Clean and modify data

**Example:**

* Copy data from SQL Server to Azure SQL

---

#### 6.1.2 Pipelines and Activities

* Pipeline: Group of activities
* Activity: Single task (copy, transform)

---

### 6.2 Azure SQL Database

A fully managed **relational database (PaaS)**.

**Why it is used:**

* Automatic backups
* High availability
* No server management

**Example:**

* Application backend database

---


