# Dual Job Date Infrastructure

## Introduction

This project contains the infrastructure code for the dual job date project. The infrastructure is a kubernetes cluster and the code contains all the neccessary files to deploy the [.NET backend](https://github.com/FH-JOANNEUM-MSD/dual-job-date-api) and the [Angular web application](https://github.com/FH-JOANNEUM-MSD/dual-job-date-web)

```bash
.
├── base
│   ├── backend
│   │   ├── deployment.yaml //dual job date api deployment
│   │   └── service.yaml //dual job date api service
│   │── frontend
│   │   ├── deployment.yaml //dual job date web deployment
│   │   └── service.yaml //dual job date web service
│   └── kustomization.yaml //kustomization file for base environment
└── overlays
    ├── development
    │   └── kustomization.yaml //kustomization file for development environment
    ├── integration
    │   └── kustomization.yaml //kustomization file for integration environment
    └── production
        └── kustomization.yaml //kustomization file for production environment


```

## Prerequisites

- [Docker](https://www.docker.com/)
- [Kubernetes](https://kubernetes.io/)
