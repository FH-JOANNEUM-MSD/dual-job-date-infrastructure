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
    │   ├── frontend
    │   │       └── ingress.yaml //ingress file for integration environment
    │   └── kustomization.yaml //kustomization file for integration environment
    └── production
        └── kustomization.yaml //kustomization file for production environment


```

## Prerequisites

- [Kubernetes](https://kubernetes.io/)

## Getting Started

1. Clone the repository
2. Change directory to the repository
3. Login to the kubernetes cluster and change to the correct namespace
4. Run the following command to deploy the infrastructure to the kubernetes staging cluster

```bash
kubectl apply -k overlays/integration
```
