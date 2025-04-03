                                                                   ## K8s ARCHITECTURE
![Kubernetes-architecture-diagram-1-1](https://github.com/user-attachments/assets/eb043f56-0b83-4f36-b74c-f8f6c7292188)

CONSIST OF 2 component

WORKER NODE 
CONTROL PLANE

ETCD CLUSTER
CONTROLLER MANAGER
SCHEDULER
API SERVER
KUBE_PROXY
KUBELET
POD
CONTAINER RUNTIME

```bash
ETCD Cluster: A distributed key-value store for storing Kubernetes cluster data.

Controller Manager: Manages controllers to ensure the desired state of the cluster (e.g., scaling, healing).

Scheduler: Assigns newly created pods to nodes based on resource availability.

API Server: The entry point for all Kubernetes operations, exposing the Kubernetes API.

Kube-Proxy: Manages network traffic routing to services and pods in the cluster.

Kubelet: Ensures containers in pods are running and healthy on each node.

Pod: The smallest deployable unit in Kubernetes, typically consisting of one or more containers.

Container Runtime: Software responsible for running and managing containers (e.g., Docker, containerd).
```
