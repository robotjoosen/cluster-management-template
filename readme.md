# Cluster Management with ArgoCD

This repository part of a cluster setup consisting of a management and git-ops repository.

- [Cluster Management](https://github.com/robotjoosen/cluster-management-template)
- [Git-ops Kustomize Repository](https://github.com/robotjoosen/gitops-kustomize-template)

# Services

| Service              | URL                                                                       | Documentation                             |
|----------------------|---------------------------------------------------------------------------|-------------------------------------------|
| ArgoCD Dashboard     | [argocd.svc.localhost](http://argocd.svc.localhost)                       | https://argo-cd.readthedocs.io/en/stable/ |
| Grafana Dashboard    | [grafana.monitoring.localhost](http://grafana.monitoring.localhost)       | https://grafana.com/                      |
| Prometheus Dashboard | [prometheus.monitoring.localhost](http://prometheus.monitoring.localhost) | https://prometheus.io/                    |

# Add-ons

- [ArgoCD Image Updater](https://argocd-image-updater.readthedocs.io/en/stable/)
- [Sealed Secrets](https://github.com/bitnami-labs/sealed-secrets)
- [Telepresence](https://www.telepresence.io/)
- [Traefik Ingress](https://doc.traefik.io/traefik/)

# Getting started (locally)

The goal of this repository is to get quickly up and running with a local development cluster. Therefor this guide is aimed
on settings up a environment with Docker Desktop and Minikube.

## Requirements

- [Docker Desktop](https://docs.docker.com/desktop/install/mac-install/)
- [Minikube](https://minikube.sigs.k8s.io/docs/start/)
- [Helm](https://helm.sh/docs/intro/install/)
- [Telepresence](https://www.telepresence.io/docs/latest/quick-start/)
- [SSHFS](https://www.getambassador.io/docs/telepresence/latest/troubleshooting#volume-mounts-are-not-working-on-macos)

## Boot up cluster

```shell
sh bin/minikube
```
