# Argo CD
[Argo CD](https://argo-cd.readthedocs.io/en/stable/) is a declarative, GitOps continuous delivery tool for Kubernetes.

## Installation
```console
helm repo add argo https://argoproj.github.io/argo-helm
helm repo update
helm search repo argo
helm show values argo/argo-cd > values.yaml
kubectl create namespace argocd
helm install --values values.yaml argocd argo/argo-cd --namespace argocd
kubectl apply -f certificate.yaml
kubectl apply -f ingress.yaml
```
