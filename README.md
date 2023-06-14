# actions-aks-namespace

Sample GitHub Action workflows showing how to securely connect to an AKS namespace.

This repository demonstrates how you can utilize GitHub Actions and OpenID Connect (OIDC) to secure connect to an Azure Kubernetes cluster that is shared across many individuals teams. In this model, each application or team would have a separate Kubernetes namespace. By leveraging RBAC we can assign permissions at the namespace level to an individual GitHub repository or environment. The workflows shown will access 2 different namespaces and list the pods in each. It also attempts to access other namespaces and will fail due to access restrictions.

For Azure RBAC enabled AKS clusters: [link](aad-rbac.md)

For Kubernetes RBAC enabled AKS clusters: [link](k8-rbac.md)
