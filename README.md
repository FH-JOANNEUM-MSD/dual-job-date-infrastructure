# Dual Job Date Infrastructure

## Introduction

This project contains the infrastructure code for the dual job date project. The infrastructure is a kubernetes cluster and the code contains all the neccessary files to deploy the [.NET backend](https://github.com/FH-JOANNEUM-MSD/dual-job-date-api) and the [Angular web application](https://github.com/FH-JOANNEUM-MSD/dual-job-date-web)

```bash
.
├── base
│   ├── backend
│   │   ├── deployment.yaml
│   │   └── service.yaml
│   │── frontend
│   │   ├── kustomization.yaml
│   │   └── deployment.yaml
│   └── kustomization.yaml
└── overlays
    ├── development
    │   └── kustomization.yaml
    ├── integration
    │   └── kustomization.yaml
    └── production
        └── kustomization.yaml


```

## Prerequisites

- [Docker](https://www.docker.com/)
- [Kubernetes](https://kubernetes.io/)
