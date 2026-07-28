# Troubleshooting Guide

Use this guide when local setup, Azure authentication, Terraform provisioning,
or application dependencies fail. It complements the deployment template and
links to the repository's complete troubleshooting reference.

## Common issue categories

| Area | Typical issues |
| --- | --- |
| Local setup | Python not found, virtual environment creation, or package installation failures. |
| Azure access | Azure CLI sign-in, Microsoft Entra authentication, permissions, and service connectivity. |
| Infrastructure | Provider configuration, resource conflicts, Terraform state locks, and quota limits. |
| Recovery | Verbose logging, Azure Service Health checks, cleanup, and retry guidance. |

!!! tip "Start with the deployment inputs"
    Confirm the selected subscription, regions, and values in the [Terraform
    deployment template](../deployment/terraform.md) before troubleshooting a
    resource-creation failure.

Open the [full troubleshooting guide](https://github.com/Cloud2BR-MSFTLearningHub/Agentic-AI-Media-Assistant/blob/main/TROUBLESHOOTING.md) for the complete issue-by-issue resolution steps.