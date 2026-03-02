# Deployment of Multi-tier (WordPress + MySQL) application in Kubernetes Cluster

**Objective:** To deploy a multi-tier MySQL application using Kubernetes with specific configurations for user roles, storage, service verification, namespace restrictions, quota limits, and data management.

**Real-time scenario:** Karen is a DevOps engineer at a tech startup. Her team has developed a new application using MySQL. Now, it is her task to deploy that application. The company plans to utilize Kubernetes for its robust container orchestration capabilities. Karen must create a Kubernetes dashboard with specific configurations, user roles, storage, service verification, and data management.

**Major Tools, Environment Used in This Project:**

- kubeadm
- kubectl
- kubelet
- Containerd
- Kubernetes Dashboard
- NFS Server

**Pre-requisites:** A Kubernetes cluster should already be set up with 3 Nodes (1 Master and 2 Worker Nodes) using kubeadm.

**High Level Diagram:**
----------------------------------------------------------------------------------------------------------------------------------

<img width="931" height="648" alt="image" src="https://github.com/user-attachments/assets/82f65baa-72e3-4106-ad72-702605de6156" />

----------------------------------------------------------------------------------------------------------------------------------

**High Levels Tasks/Steps:**

-	Create Kubernetes Dashboard
-	Install & Configure NFS Server, create NFS based PV & PVC
-	Create Secret for MySQL Deployment
-	Create Deployment for MySQL (attach PV, PVC)
-	Create ConfigMap and Secret for Wordpress Deployment
-	Create Deployment for Wordpress (PV not required)
-	Expose Service for WordPress and MySQL Deployment
-	Verify the Deployment of Application on web browser
-	Verify the Cluster and its workloads on Kubernetes Dashboard


