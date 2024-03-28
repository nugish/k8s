# Cert-Manager
[cert-manager](https://cert-manager.io/)  adds certificates and certificate issuers as resource types in Kubernetes clusters, and simplifies the process of obtaining, renewing and using those certificates.

It can issue certificates from a variety of supported sources, including Let’s Encrypt, HashiCorp Vault, and Venafi as well as private PKI.

## Installation
```console
helm repo add jetstack https://charts.jetstack.io --force-update
helm repo update
helm install cert-manager jetstack/cert-manager \
--namespace cert-manager \
--create-namespace \
--version v1.14.4 \
--set installCRDs=true

kubectl create ns sandbox
kubectl apply -f issuer-self-certificate.yaml  
```

