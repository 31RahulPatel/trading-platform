# Infrastructure Directory

This directory contains Infrastructure as Code (IaC) configurations:

## Terraform (`terraform/`)
- AWS infrastructure provisioning
- EKS cluster setup
- VPC, subnets, security groups
- RDS, ElastiCache, ALB configuration

## Kubernetes (`k8s/`)
- **`base/`** - Base Kubernetes manifests
- **`overlays/staging/`** - Staging environment configs
- **`overlays/production/`** - Production environment configs
- **`argocd/`** - ArgoCD application definitions

## Usage
```bash
# Terraform
cd terraform/
terraform init
terraform plan
terraform apply

# Kubernetes
kubectl apply -f k8s/overlays/staging/
```