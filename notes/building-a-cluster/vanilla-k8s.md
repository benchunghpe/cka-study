# Vanilla Kubernetes

## Understanding Vanilla Kubernetes
- Released open-source every four months, installed with kubeadm
- Has core functionality, no networking, support or GUI
- Need external tools for additional functionality

## Understanding the Ecosystem.
- CNCF hosts many projects for cloud native computing
- Projects for Networking, dashboard, storage, observability, ingress

## Kubernetes distributions
- Kubernetes add products from the ecosystem to vanilla Kubernetes and add support.
- Normally distributions are a version or two behind
- Some distributions only support one solution

### Cloud distributions
- EKS
- AKS
- GKE

### On-prem distributions
- Openshift
- Google Antos
- Rancher
- Canonical Charmed Kubernetes

### Learning solutions
- Minikube
- K3s

# Kubernetes node roles
- Control plane runs core services, agents, and no user workloads
- Worker plane run user workloads
- All nodes require a container runtime 
- Kubelet systemd service is responsible for running orchestrated containers as pods on any nodes

## Node structure
### Control node
Reach out using kubectl on the control node
---
calico
---
- request from apiserver is stored in...
- etcd (stores resources) which then received by the
- scheduler which gets in touch with the kubelet 
--- 
- CRI - container runtime
- Kublet

### Worker node
myapp

calico
--- 
- CRI - container runtime
- Kublet
