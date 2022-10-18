# Kubernetes (K8s) Practice
12 week routine of practice and implementation details

## WEEK 1
### Practice creating a cluster
- [Kubernetes the hard way](https://github.com/kelseyhightower/kubernetes-the-hard-way)
- [Create local cluster with kind](https://youtu.be/m-IlbCgSzkc)
- [create local cluster with minikube](https://youtu.be/E2pP1MOfo3g)
- [Use kubeadm to create a K8s cluster on Ubuntu](https://www.digitalocean.com/community/tutorials/how-to-create-a-kubernetes-cluster-using-kubeadm-on-ubuntu-20-04)

## WEEK 2

- [Free courses on ACG Oct 2022](https://acloudguru.com/blog/news/whats-free-at-acg)
- [Creating user and role in K8s](https://killercoda.com/chadmcrowell/scenario/kubernetes-create-user)
- [How HTTPS works](https://youtu.be/T4Df5_cojAs)
- [PKI - part 1](https://youtu.be/aCDgFH1i2B0)
- [PKI - part 2](https://youtu.be/Jefr7wFLu3M)
- [Chapter 1 - Section 6](https://youtu.be/1Aq4RRq32gM)

### CHALLENGES

> Put all YAML files in WEEK2 directory

1. Create the YAML for a certificate signing request.
2. Create the YAML for a `role` named "pod-reader" that allows users to perform get, watch and list on pods.
3. Create the YAML for a `roleBinding` named "admin-binding", in the namespace "acme", granting permissions for the "admin" ClusterRole to a user named "bob".

## WEEK 3

- [VIDEO: Create custom image and push to DockerHub](https://youtu.be/_H6X96dvqBw)
- [VIDEO: Deployment vs. StatefulSet](https://youtu.be/pPQKAR1pA9U)
- [VIDEO: Pods and Containers](https://youtu.be/5cNrTU6o3Fw)
- [VIDEO: Pod Lifecycle](https://youtu.be/wlYESb124xM)
- [VIDEO: Create Pods & Deployment](https://youtu.be/7bA0gTroJjw)
### CHALLENGES

> Put all YAML files in WEEK3 directory

1. Take the image that you built in the first video above and deploy it as a pod in Kubernetes
2. Create a deployment with the image used in the previous challenge and scale it to 5 replicas
3. Create a second deployment that uses the image "mysql:8" and include an environment variable that is the MYSQL default password

## WEEK 4

- [VIDEO: What is Helm and Helm Charts](https://youtu.be/-ykwb1d0DXU)
- [VIDEO: Introduction to Helm](https://youtu.be/5_J7RWLLVeQ)
- [VIDEO: Hands on w/Helm](https://youtu.be/6d6L4-ADF-M)
- [Helm Quickstart](https://helm.sh/docs/intro/quickstart/)
- [The Big Three Concepts](https://helm.sh/docs/intro/using_helm/)
- [Helm Tutorial](https://www.freecodecamp.org/news/what-is-a-helm-chart-tutorial-for-kubernetes-beginners/)
- [Helm vs. Kustomize](https://harness.io/blog/helm-vs-kustomize)

### CHALLENGES

> Put all YAML files in WEEK4 Directory

1. Install the nginx ingress controller nginx-stable via https://helm.nginx.com/stable
2. Install Hashicorp Vault via helm chart `hashicorp/vault` at https://helm.releases.hashicorp.com
3. Override the values file for vault using the default here: https://github.com/hashicorp/vault-helm/blob/main/values.yaml
4. Create a helm chart from scratch and deploy it to Kubernetes

## WEEK 5

## WEEK 6

## WEEK 7

## WEEK 8

## WEEK 9

## WEEK 10

## WEEK 11

## WEEK 12
