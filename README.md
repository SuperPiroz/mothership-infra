# mothership-infra

Infrastruktur som kod (IaC), Kubernetes-manifest och driftkonfiguration för **Mothership Dashboard**.

## Innehåll
- `docker-compose.yml` – Lokal utvecklingsmiljö för att köra alla mikrotjänster och databaser lokalt med ett enda kommando.
- `k8s/` – Kubernetes-manifest för k3s på hemmaservern (Deployments, Services, Ingress, NetworkPolicies, RBAC).
- `policies/` – Policy as Code med Kyverno / OPA Conftest (containersäkerhet, non-root, godkända register).
- `backup/` – CronJob för nattlig databasbackup till Backblaze B2 (S3).
