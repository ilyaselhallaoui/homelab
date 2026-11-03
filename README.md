# homelab

My Kubernetes homelab: K3s with a VPS as the control plane and my old laptop as the worker. This is where I practise what I learn: DevOps, cloud and running AI.

**Status:** paused since 2026-10-21.

## Setup

| Role | Machine | Runs |
|---|---|---|
| Control plane | VPS | Ubuntu, K3s server |
| Worker | old laptop | Ubuntu, K3s agent |

The nodes are connected over Tailscale.

## What's in this repo

| Path | What it is |
|---|---|
| [`Basics/`](Basics/) | Single-pod manifests from going back to the Kubernetes basics: nginx, whoami, Homarr, Pi-hole, Uptime Kuma. |

## Earlier work

Before the restructure in June 2026 the repo held full app setups (namespace, PV/PVC, deployment, service, ingress) for Firefly III, Homarr, Jellyfin, Pi-hole, wger and a Prometheus/Grafana/Alertmanager monitoring stack installed with Helm. They are still in the git history at commit [`bfdda7a`](https://github.com/ilyaselhallaoui/homelab/tree/bfdda7a).

## Secrets

Real secrets stay out of this repo: `.gitignore` excludes `.env` files and secret manifests.

## More

I write about what I build on my website, [Desired State](https://fsh-ilyas-website.ilyas-elhallaoui.workers.dev/en/).
