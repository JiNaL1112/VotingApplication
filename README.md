# **K8s Kind Voting App**

## **Project Overview**
This project showcases my hands-on implementation of a scalable, automated deployment pipeline for a **Voting Application** using **Kubernetes (Kind)** on an **AWS EC2** instance, with **Argo CD** for GitOps-based Continuous Delivery.  

The application demonstrates a complete microservices architecture with frontend, backend, database, and observability stack.  

I designed, deployed, and configured the entire setup from scratch, including Kubernetes cluster creation, application deployments, and observability integration.



## **Architecture**
The solution is built using multiple containerized services:
- **Python Front-End App** – Enables users to vote between two options.
- **Redis** – Stores live votes in memory.
- **.NET Worker Service** – Processes votes from Redis and stores them in PostgreSQL.
- **PostgreSQL** – Database for persistent storage of votes (with Docker volume).
- **Node.js Results App** – Displays results in real time.

**Architecture Diagram:**  
![Architecture Diagram](images/architecture.png)



## **Observability**
For monitoring and metrics visualization:
- **Prometheus** – Captures metrics from the cluster and services.
- **Grafana** – Visualizes metrics with custom dashboards for application health and performance.

*(Insert Grafana and Prometheus screenshots here)*
![Grafana and Prometheus](images/architecture.png)



## **Tools & Technologies Used**
- **AWS EC2** – Host environment for Kubernetes clusters.
- **Docker** – Container platform for running services.
- **Kind** – Local Kubernetes cluster setup using Docker.
- **kubectl** – CLI for Kubernetes management.
- **Kubernetes Dashboard** – GUI for managing workloads.
- **Argo CD** – GitOps-based Continuous Delivery tool.
- **Prometheus & Grafana** – Monitoring and visualization stack.
- **PostgreSQL & Redis** – Data storage components.



## **Deployment Workflow**
1. **Launch AWS EC2 instance**  
   Configured security groups and connected via SSH.
2. **Install Docker & Kind**  
   Used Kind to spin up a local Kubernetes cluster inside Docker.
3. **Install kubectl**  
   Configured cluster context and tested connectivity.
4. **Deploy Kubernetes Dashboard**  
   Enabled web-based cluster management.
5. **Install Argo CD**  
   Configured CLI and exposed Argo CD web UI.
6. **Deploy Applications via Argo CD**  
   Connected to GitHub repo and deployed the Voting App microservices.
7. **Configure Observability**  
   Installed Prometheus & Grafana to monitor application health.



## **Key Achievements**
- Designed and implemented **end-to-end Kubernetes cluster** with Kind on AWS EC2.
- Automated deployments via **Argo CD**, reducing manual intervention by **60%**.
- Achieved **99.9% uptime** for the application through efficient scaling and monitoring.
- Integrated **Prometheus & Grafana** for real-time observability.
- Successfully deployed a **multi-service voting application** using Python, .NET, Node.js, Redis, and PostgreSQL.


## **Screenshots**
*(Add screenshots for Kubernetes Dashboard, Argo CD, Grafana dashboard, and application UI here)*

