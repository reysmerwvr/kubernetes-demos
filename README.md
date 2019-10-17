
# kubernetes-demos

Learn DevOps: The Complete Kubernetes Course.

## Requirements

- Kubernetes
- minikube >= 1.3.1
- kubectl >= 1.15.0

## Version

1.0.0

## Installation

Download zip file and extract it [latest pre-built release](https://github.com/reysmerwvr/kubernetes-demos). Or clone the repository and cd into it.

This project uses a number of open source projects to work properly:

- [Kubernetes] - Production-Grade Container Orchestration

## Setup

Install kubectl and minikube for your OS.

[macOS](https://kubernetes.io/docs/tasks/tools/install-kubectl/#install-kubectl-on-macos)
[Windows](https://kubernetes.io/docs/tasks/tools/install-kubectl/#install-kubectl-on-windows)
[Linux](https://kubernetes.io/docs/tasks/tools/install-kubectl/#install-kubectl-on-linux)

## Run minikube

```bash
hyperv
$ minikube start --vm-driver hyperv --hyperv-virtual-switch "<Minikube Name>"
virtualbox
$ minikube start –vm-driver=virtualbox -p <name>
```

Once running minikube

```bash
cd kubernetes-demos
minikube status
kubectl cluster-info
kubectl apply -f <demo-name>/
```

To verify pods/services status

```bash
cd kubernetes-demos
kubectl get pods
kubectl get services
```

To verify minikube ip

```bash
cd kubernetes-demos
minikube ip
```

### Todos

- Add code comments

[//]: # "These are reference links used in the body of this note and get stripped out when the markdown processor does
its job. There is no need to format nicely because it shouldn't be seen. Thanks SO - http://stackoverflow.com/questions/4823468/store-comments-in-markdown-syntax"
[Kubernetes]: https://kubernetes.io/