# DevOps Assessment - ArgoCD Configuration

## ApplicationSet Overview

This repository contains ArgoCD ApplicationSet configurations for deploying a Spring Boot API across multiple environments.

### Configuration Details

The ApplicationSet is configured to deploy the application to:
- Development environment (`dev-global-cluster-0`)
- Production environment (`prd-global-cluster-5`)

### Key Features
- Automated sync enabled
- Prune and self-heal capabilities
- Environment-specific value files
- Helm chart deployment

### Directory Structure
```
├── argocd/
│   └── application-set.yaml    # Main ApplicationSet configuration
```

## Usage

The ApplicationSet will automatically create ArgoCD Applications for each environment defined in the generator list. Each application will:
- Use environment-specific value files
- Deploy to designated clusters
- Maintain sync with the source repository

## Prerequisites
- ArgoCD installed in the cluster
- Access to the Helm chart repository
- Kubernetes cluster access
