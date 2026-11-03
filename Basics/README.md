# Basics

Single-pod manifests for learning the Kubernetes building blocks before running real apps. They are plain `Pod` objects without a Deployment, Service or Ingress, so they are for practice, not for running anything long-term.

| Manifest | Image | Namespace |
|---|---|---|
| `pods/nginx.yaml` | `nginx` | `basics` |
| `pods/whoami.yaml` | `traefik/whoami` | `basics` |
| `pods/pihole.yaml` | `pihole/pihole:latest` | `basics` |
| `pods/uptime-kuma.yaml` | `louislam/uptime-kuma:nightly2` | `basics` |
| `pods/homarr.yaml` | `ghcr.io/homarr-labs/homarr:latest` | none set, uses the current namespace |

## Apply

```bash
kubectl create namespace basics
kubectl apply -f Basics/pods/
kubectl -n basics get pods
```
