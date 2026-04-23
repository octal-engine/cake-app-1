# Documents for cake-app-1

This is a template app!

For fun, it shows you a random dev excuse + a random cat

# How to access the app?

You can access the app by accessing this URL: `cake-app-1-prod.gabrieleweka.dev`

# Extra info?

This application has two API endpoints:

- `/api/v1/info`
- `/api/v1/healthz`

Here you could expand on what each of these endpoints do.

---

# Platform URLs & Credentials

All infrastructure is publicly reachable. Credentials below are read-only (safe to share). For admin access, ping **@Eweka01**.

| Service | URL | Auth |
|---|---|---|
| **Backstage** (this portal) | https://backstage.gabrieleweka.dev | Sign in with GitHub |
| **ArgoCD** | https://argocd.gabrieleweka.dev | `viewer` / `viewer123` (read-only) |
| **Grafana** | http://grafana.gabrieleweka.dev | No login needed (anonymous Viewer) |
| **Prometheus** | http://prometheus.gabrieleweka.dev | No auth |
| **This app's repo** | https://github.com/octal-engine/cake-app-1 | GitHub |
| **This app's CI** | https://github.com/octal-engine/cake-app-1/actions | GitHub |
| **Docker image** | `eweka/cake-app-1:<commit-sha>` | public on Docker Hub |

## ArgoCD read-only scope

The `viewer` account can **see** applications, repos, projects, and pod logs, but **cannot create, sync, or delete** anything. Safe to share for demos.

## Grafana dashboards worth looking at

- **Kubernetes / Compute Resources / Namespace (Pods)** — per-namespace CPU/memory
- **Node Exporter / Nodes** — host-level metrics for the kind cluster
- **CoreDNS** — DNS inside the cluster
