# kubernetes-journey

Udemy course: https://www.udemy.com/course/learn-kubernetes/

Used technologies:
- Docker: Used to run the Minikube container for local Kubernetes cluster.
- Minikube: Used to create a local Kubernetes cluster.
- Kubectl: Used to manage and interact with the Kubernetes cluster.

## 6_Voting_App:

### Voting app: http://104.154.129.18/

### Result app: http://35.224.182.195/

**NodePort: Exposes the service on a specific port on each node (Voting App and Result App)**

**ClusterIP: Exposes the service internally within the cluster (Redis and Postgres)**

![image](https://github.com/user-attachments/assets/27822b29-fffd-4452-a9bd-4eae5643421a)

## Voting app deployed to GCP using Kubernetes cluster (NodePorts were replaced with LoadBalancers):

![image](https://github.com/user-attachments/assets/a777187b-d9c4-4cab-8d0f-6cce87d6e146)

![image](https://github.com/user-attachments/assets/c27a8e27-9140-4f62-a086-5bf2760e7b5e)

## Summary:

Pod: A group of one or more containers that are deployed together on the same host.

ReplicaSet: Ensures a specified number of pod replicas are running at any given time.

Deployment: A higher-level abstraction for managing ReplicaSets and ensuring the desired state of applications.

Service Types:
* NodePort: Exposes the service on a specific port on each node.
* ClusterIP: Exposes the service internally within the cluster.
