# ☸️ Kubernetes Microservices Platform with Monitoring

A production-style microservices application deployed on **Kubernetes** with **Prometheus** and **Grafana** for monitoring and visualization.

This project demonstrates container orchestration, service discovery, scaling, and real-time monitoring of a distributed application using Kubernetes.

---

# 📌 Project Overview

This project deploys a **Voting Application** built using a microservices architecture on Kubernetes.

The platform consists of multiple independent services that communicate with each other while Kubernetes manages deployment, networking, scaling, and availability. Prometheus collects application and cluster metrics, and Grafana provides interactive dashboards for monitoring system health.

---

# 🏗️ Architecture

```text
                    User
                      │
                      ▼
              Voting Web App
                      │
         ┌────────────┴────────────┐
         ▼                         ▼
      Redis                     PostgreSQL
         │                         ▲
         ▼                         │
      Worker Service ──────────────┘
                      │
                      ▼
              Result Web App

────────────────────────────────────────

           Kubernetes Cluster
      ├── Deployments
      ├── Services
      ├── ConfigMaps
      ├── Persistent Volumes
      └── Horizontal Scaling

────────────────────────────────────────

        Monitoring Stack

     Prometheus ─────► Grafana
```

---

# 🚀 Features

* Microservices-based Voting Application
* Kubernetes Deployments and Services
* Containerized using Docker
* Service discovery within Kubernetes
* Prometheus metrics collection
* Grafana dashboards for visualization
* Horizontal application scaling
* High availability using Kubernetes
* Persistent storage for database
* Easy deployment using Kubernetes manifests

---

# 🛠️ Tech Stack

| Category         | Technologies |
| ---------------- | ------------ |
| Containerization | Docker       |
| Orchestration    | Kubernetes   |
| Monitoring       | Prometheus   |
| Visualization    | Grafana      |
| Cache            | Redis        |
| Database         | PostgreSQL   |
| Version Control  | Git & GitHub |
| Operating System | Linux        |

---

# 📂 Project Structure

```text
.
├── voting-app/
├── result-app/
├── worker/
├── k8s/
│   ├── deployments/
│   ├── services/
│   ├── configmaps/
│   ├── persistent-volumes/
│   └── monitoring/
├── prometheus/
├── grafana
└── README.md
```

---

# ⚙️ Kubernetes Components

The application uses the following Kubernetes resources:

* Deployments
* Services
* ConfigMaps
* Persistent Volumes (PV)
* Persistent Volume Claims (PVC)
* Namespaces
* ReplicaSets
* Pods

---

# 📊 Monitoring Stack

### Prometheus

Prometheus is used to:

* Collect Kubernetes metrics
* Monitor application performance
* Monitor resource utilization
* Track pod health

### Grafana

Grafana provides dashboards for:

* CPU usage
* Memory utilization
* Pod status
* Node health
* Application metrics
* Kubernetes cluster monitoring

---

# 🚀 Deployment

## Clone Repository

```bash
git clone https://github.com/your-username/your-repository.git

cd your-repository
```

## Deploy Kubernetes Resources

```bash
kubectl apply -f k8s/
```

## Verify Deployments

```bash
kubectl get all
```

## Check Running Pods

```bash
kubectl get pods
```

## Check Services

```bash
kubectl get svc
```

---

# 📈 Scaling the Application

Increase the number of application replicas:

```bash
kubectl scale deployment voting-app --replicas=3
```

Verify:

```bash
kubectl get pods
```

---

# 📊 Monitoring

Access Prometheus and Grafana after deployment.

Typical monitoring includes:

* Cluster health
* Pod metrics
* CPU and memory utilization
* Application response metrics
* Resource consumption
* Service availability

---


---

# 🎯 Skills Demonstrated

* Kubernetes Administration
* Microservices Architecture
* Docker Containerization
* Kubernetes Deployments
* Service Discovery
* Application Scaling
* Monitoring with Prometheus
* Dashboard Creation using Grafana
* Linux
* Git & GitHub

---






