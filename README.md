## aws-projects
### Overview

This project demonstrates an enterprise-style DevSecOps pipeline integrating infrastructure-as-code, containerized workloads, CI/CD security gates, and policy-as-code enforcement.

### Security Controls

- Infrastructure scanning via Checkov
- Container vulnerability scanning via Trivy
- Policy enforcement via OPA
- CI/CD gates to block insecure deployments

### Architecture

- AWS VPC and EC2 deployed via Terraform
- Docker based web application
- GitHub Actions for CI/CD automation

### Threat Model

- Publicly exposed infrastructure
- Excessive IAM permissions
- Vulnerable container images

### Cost Controls

Infrastructure was designed to remain within AWS Free Tier only and avoid NAT gateways, load balancers, and large data transfers.