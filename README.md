# 🌟 Kustomize Kubernetes Configurations 🚀

Welcome to the **Kustomize Kubernetes Configurations** repository! This repo is designed to simplify the management and deployment of Kubernetes resources using Kustomize.
## 🚀 Features

- **Base & Overlay Structure**: Manage shared resources and environment-specific configurations seamlessly.
- **Environment Flexibility**: Easily add new environments such as `staging`, `prod`, etc.
- **Customizable & Scalable**: Patch and customize your deployments without duplicating resources.

## 🧑‍💻 Directory Structure

Here’s how the repository is structured:

```plaintext
k8s-kustomize/
│── apps/
│   └── kustomization.yaml          # Application-level common configurations
│
├── base/
│   ├── deployment.yaml            # Base deployment configuration
│   ├── kustomization.yaml         # Base kustomization file for common resources
│   ├── service.yaml               # Base service configuration
│
└── overlays/
    └── dev/
        ├── deployment-patch.yaml  # Dev-specific patch for the deployment
        └── kustomization.yaml     # Dev-specific Kustomize file
