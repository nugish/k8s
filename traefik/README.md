# Traefik
[Traefik](https://traefik.io/traefik/) is a leading modern reverse proxy and load balancer that makes deploying microservices easy.

## Installation
```console
helm repo add traefik https://traefik.github.io/charts
helm repo update
helm install traefik traefik/traefik -n traefik --create-namespace
kubectl apply -f certificate.yaml
kubectl apply -f dashboard.yaml
```

