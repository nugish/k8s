# Pgadmin
[pgadmin4](https://traefik.io/traefik/) is web based administration tool for PostgreSQL database.

## Installation
```console
helm repo add runix https://helm.runix.net
helm repo update
helm install pgadmin runix/pgadmin4
kubectl apply -f certificate.yaml
kubectl apply -f ingress.yaml
```

## Add Service for External PostgreSQL Database
```console
kubectl apply -f postgresql-service.yaml
```
