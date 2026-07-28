# Terraform Deployment Template

Use the repository Terraform template to provision the Azure infrastructure,
create the configured Foundry resources and agents, and deploy the application.

!!! warning "Review values before applying"
    The supplied `terraform.tfvars` is a demo configuration. Review regions,
    resource names, model availability, quotas, and subscription constraints
    before running an apply in your environment.

## Template files

| File | Purpose |
| --- | --- |
| [main.tf](https://github.com/Cloud2BR-MSFTLearningHub/Agentic-AI-Media-Assistant/blob/main/terraform-infrastructure/main.tf) | Defines the infrastructure resources and their relationships. |
| [variables.tf](https://github.com/Cloud2BR-MSFTLearningHub/Agentic-AI-Media-Assistant/blob/main/terraform-infrastructure/variables.tf) | Declares the configurable template inputs. |
| [terraform.tfvars](https://github.com/Cloud2BR-MSFTLearningHub/Agentic-AI-Media-Assistant/blob/main/terraform-infrastructure/terraform.tfvars) | Provides the demo deployment values to adapt for your environment. |
| [provider.tf](https://github.com/Cloud2BR-MSFTLearningHub/Agentic-AI-Media-Assistant/blob/main/terraform-infrastructure/provider.tf) | Configures Terraform providers. |
| [outputs.tf](https://github.com/Cloud2BR-MSFTLearningHub/Agentic-AI-Media-Assistant/blob/main/terraform-infrastructure/outputs.tf) | Exposes the resulting resource and application details. |

## Deploy

1. Review and update the [Terraform variable template](https://github.com/Cloud2BR-MSFTLearningHub/Agentic-AI-Media-Assistant/blob/main/terraform-infrastructure/terraform.tfvars).
2. Sign in with `az login` and select the target subscription.
3. Run `terraform init`, then review `terraform plan -var-file terraform.tfvars`.
4. Apply the approved plan with `terraform apply -var-file terraform.tfvars`.

For prerequisites, screenshots, and the full provisioning procedure, open the
[Terraform deployment guide](https://github.com/Cloud2BR-MSFTLearningHub/Agentic-AI-Media-Assistant/blob/main/terraform-infrastructure/README.md).