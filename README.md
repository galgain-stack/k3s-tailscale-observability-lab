# 🧩 k3s Tailscale Observability Lab

## 📌 Overview
This project demonstrates building a **multi-node k3s Kubernetes cluster** using **Tailscale** for secure networking, with **Prometheus and Grafana** for monitoring and observability.

---

## 🏗️ Architecture

- **Control Plane**
  - `masterhome`

- **Worker Nodes**
  - `worker1`
  - `worker2`

- **Networking**
  - Tailscale (100.x.x.x private mesh network)

- **Monitoring Stack**
  - Prometheus (metrics collection)
  - Grafana (visualization)
  - Node Exporter (per-node metrics)

---

## 🔧 Technologies Used

- Kubernetes (k3s)
- Tailscale (WireGuard-based networking)
- Prometheus
- Grafana
- Linux (Ubuntu)

---

## 🚀 Key Features

- Multi-node Kubernetes cluster
- Secure node-to-node communication using Tailscale
- Real-time monitoring with Prometheus
- Grafana dashboards for cluster visibility
- Node-level metrics across all workers

---

## 📊 Monitoring

Grafana dashboards used:
- Kubernetes / Compute Resources / Cluster
- Kubernetes / Compute Resources / Node
- Kubernetes / Networking / Cluster

---

## 📸 Screenshots

_(Add screenshots here)_

Example:
```
![Cluster Dashboard](screenshots/cluster-dashboard.png)
```

---

## ⚠️ Security Notes

- Sensitive data (tokens, kubeconfig, credentials) are not included
- Access controlled via Tailscale
- SSH access limited to authorized users

---

## 🔮 Future Improvements

- Migrate from Tailscale to native WireGuard
- Implement Kubernetes RBAC for multi-user access
- Add persistent storage for Prometheus
- Deploy sample applications across nodes
- Implement alerting (CPU/memory thresholds)

---

## 🧠 Lessons Learned

- Kubernetes node identity is tied to hostname
- Proper IP selection is critical in multi-network setups
- Tailscale simplifies secure cluster networking
- Observability is essential for understanding cluster behavior

---
