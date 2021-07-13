# Notes for Kubernetes k8s exams

Below are a list of notes for preparing for CKA, CKAD, CKAS

`minikube` is by far the easiest way to get started learning Kubernetes.

- VirtualBox: a free and open-source hosted hypervisor for x86 virtualization, developed by Oracle Corporation
- Vagrant: an open-source software product for building and maintaining portable virtual software development environments; e.g., for VirtualBox
- kubectl: The Kubernetes command-line tool, which allows you to run commands against Kubernetes clusters.

For MacOS, Homebrew Package Manager makes it easy to get started.

[Install Homebrew on Mac](https://brew.sh/)

## Quickstart

The following will get you started quickly with k8s on a mac.

Install

```sh
brew cask install virtualbox
brew cask install vagrant
brew install minikube
```

Deploy

```sh
# one node setup
minikube start

# three node setup w/ cri-o
minikube start --container-runtime=cri-o --nodes=3

# control docker/podman locally
eval $(minikube docker-env)
eval $(minikube podman-env)

# cleanup
minikube delete
```

Verify
```sh
kubectl get nodes
kubectl get pods --all-namespaces
```

Other Config
```sh
# use bash shell
brew install bash
dscl . -read /Users/$USER UserShell 
sudo dscl . -change /Users/$USER UserShell /bin/bash /usr/local/bin/bash

# auto complete for minikube
source <(minikube completion bash)

# auto complete for kubectl
source <(kubectl completion bash)
```
