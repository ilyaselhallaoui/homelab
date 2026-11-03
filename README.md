# homelab

My Kubernetes homelab: my old laptop, rebuilt as an Ubuntu server running K3s. This is where I practise what I learn: DevOps, cloud and running AI.

**Status:** paused since 2026-10-21, restarting soon.

## Setup

| Role | Machine | Runs |
|---|---|---|
| Node | old laptop | Ubuntu, K3s (single node) |

Remote access runs over Tailscale.

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
