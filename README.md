# My Introduction to Kubernetes (& other CICD Tools)
## Goals
This repo was created as a way to document my knowledge on emerging CICD Tools and to spark growth through self-studying.
* Kubernetes
  * [ ] Understand the Terminology (Kubernetes, Nodes/Minions, Master, Pods, etc.)
  * [ ] Getting started with tools (Using minikube, VirtualBox, kubectl via Command Prompt)
  * [ ] Create a Deployment 
  * [ ] Create a Cluster
  * [ ] Create a Loadbalancer
  * [ ] Udemy learn Kubernetes Certificate
* Docker
* Ansible

### Kubernetes
__Terminology__
| Term  | Meaning |
| ------------- | ------------- |
| Container  | A piece of software that packages code, components and its dependencies (i.e Docker, Ansible) so that it can run quickly and reliably in isolated envs.  |
| Virtual Machine vs Container  | Virtual Machines run on a hypervisor and each VM has it's own OS, libraries and dependences. Containers are installed on the OS. Containers share the same OS kernel so different flavors/softwares of Linux can be made to run on the same Linux kernel. VMs can be much slower because they have higher utilization, boot up slower, and use higher disk space.  |
| Image vs Container  | An image is like a template for a container. Once it has been deployed and is running it becomes a container.  |
| Kubernetes  | A container orchestration tool that was created by Google but is now Open-Source. It can manage the auto-scaling of loads and connectivity between hundreads of containers.   |
| Node/Minion  | A physical or virtual machine that K8s is installed on. Has the kubelet  |
| Cluster  | A group of Nodes. Can be used to share loads and to increase app reliability.  |
| Master | A node that manages slave nodes and contains logs. Has the kube-apiserver.  |
| kubectl | Kubernetes Command Line. Used to deploy and manage applications on the cluster  |

__Main Kubernetes Components__
| Component  | Role |
| API Server | The frontend of Kubernetes  |
| etcd | Key-value store that contains logs for the cluster  |
| Scheduler | Distributes work to containers  |
| Controller | Notices and responds when nodes go down and brings up new containers to address load shortages  |
| Container Runtime | The underlying software used to run containers (Docker)  |
| kubelet | The agent that runs on each node in the cluster  |

__Common Commands__
| Command  | What Does It Do? |
| `kubectl run name` | Content Cell  |
| `kubectl cluster-info` | Content Cell  |
| `kubectl get nodes` | Content Cell  |

__Creating a Deployment__

