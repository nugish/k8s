# Traefik
[Traefik](https://traefik.io/traefik/) is a leading modern reverse proxy and load balancer that makes deploying microservices easy.

## Installation
```console
helm repo add traefik https://helm.traefik.io/traefik
helm repo update
helm install traefik traefik/traefik --values traefik.yaml -n traefik --create-namespace
kubectl apply -f certificate.yaml
kubectl apply -f dashboard.yaml
```

