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

- [VIDEO: Types of Services in K8s](https://youtu.be/T4Z7visMM4E)
- [Services - K8s Documentation](https://kubernetes.io/docs/concepts/services-networking/service/)
- [EXERCISE: Use a service to expose your app](https://kubernetes.io/docs/tutorials/kubernetes-basics/expose/)
- [EXERCISE: Using Source IP](https://kubernetes.io/docs/tutorials/services/source-ip/)
- [EXERCISE: Access services running in K8s](https://killercoda.com/examples/scenario/network-traffic-kubernetes)

### CHALLENGES

> Put all the files for these exercises in the WEEK5 directory

1. Create a NodePort service in K8s that uses port 30000 on the node and port 8080 on the container
2. Only use the kubectl command-line to create a deployment named 'nginx-deploy' that uses the `nginx` image, exposed on port 80. Only 1 replica will be used. 
3. Again, only use the kubectl command-line to expose the deployment 'nginx-deploy' and use the target port of 8080.
4. Change the service named 'kubernetes' already running in the default namespace to a NodePort type service using the kubectl command line

## WEEK 6

- [VIDEO: Rolling Updates](https://youtu.be/xRifmrap7S8)
- [TUTORIAL: Scaling an App](https://kubernetes.io/docs/tutorials/kubernetes-basics/scale/scale-interactive/)
- [VIDEO: Using Set Image](https://youtu.be/RV8Avr7KEi8)

### CHALLENGES

> Put all files in WEEK6 Directory

1. Create a deployment named “apache” that uses the image httpd:2.4.54 and contains three pod replicas.
2. After the deployment has been created, scale the deployment to five replicas
3. Change the image for the "apache" deployment to httpd:alpine
4. Look at the rollout history, then go back to the previous rollout (roll back)

 
## WEEK 7

- [VIDEO: Network Policies](https://youtu.be/oBf5lrmquYI?t=944)
- [VIDEO: Network Policy & Service Mesh Differences](https://youtu.be/lHC7xpFack8?t=973)
- [VIDEO + GITHUB REPO: Network Policies](https://youtu.be/ka0C09CAfho?t=7615)
- [DOCS: Network Policies](https://kubernetes.io/docs/concepts/services-networking/network-policies/)
- [Network Policy Tutorial](https://kubernetes.io/docs/tasks/administer-cluster/declare-network-policy/)

### CHALLENGES

1. Deploy the following resources in Kubernetes: https://gist.github.com/chadmcrowell/7e5cbb782bf2b9e90c6abe8cd8cd39b0
2. Start a new pod with the image `radial/busyboxplus:curl`, get a shell to it, and run `curl http://db:15984` to try to communicate from pod to pod
3. Create a network policy that will deny all traffic from pod to pod
4. Create another network policy that applies to pods that have the label `app=db`. Allow traffic from pods that have the label `app=api` and only over port `5984`.
5. Create another network policy that applies to pods that have the label `app=web`. Allow traffic from pods that have the label `app=web` on port `3000`. Allow traffic out to pods that have the label `app=db` over port `5984`. Also allow traffic to pods in the kube-system namespace that match label `k8s-app=kube-dns` on port 53.
6. Start a new pod with the image `radial/busyboxplus:curl` and label app=api, get a shell to it, and run `curl http://db:15984` to try to communicate from pod to pod

## WEEK 8

## WEEK 9

## WEEK 10

## WEEK 11

## WEEK 12
