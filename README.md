# Employees DevOps portfolio
## GitOps config repository
This repository contains the Helm charts and all manifests required to run the "Employees" application and all other components it needs in a Kubernetes cluster.

These manifests are being managed by ArgoCD, which runs in the cluster. 
![Project architecture image](architecture.jpg)

## Components
The following components are deployed in the Kubernetes cluster:

- EFK stack for the application logging
- kube-prometheus-stack for monitoring
- ingress-nginx for exposing the application
- cert-manager for certificate management
- sealed-secret for storing secrets securely

# Additional Information
It's worth noting that this configuration repository is intended to be used in conjunction with the [source code repository](https://github.com/Daniel-Yakov/Employees) and [infrastructure repository](https://github.com/Daniel-Yakov/portfolio-infra) to provide a complete DevOps solution for the application.