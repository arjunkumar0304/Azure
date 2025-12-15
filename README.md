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

---

