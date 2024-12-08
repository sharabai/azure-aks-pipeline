# Azure DevOps pipeline.

## Description

Azure DevOps pipeline that installs Nginx Ingress controller to aks cluster, configures it to two example kubernetes applications.

## Instruction

Create a project in Azure DevOps, add service connections for this github repo, your azure subscription and aks. You can provision those resources using my Terraform IaC [repo](https://github.com/sharabai/terraform-azure-dev-ops-agent). This pipeline uses self-hosted agent, which is also provisioned at terraform repo. Terraform repo also creates Variable group that has var: "resourceGroup", "clusterName", "subscription". Create those in case you create you don't use my terraform repo.
It also assumes that Azure-Cli is available on the agent.

## License

This project is licensed under a custom restrictive license. All rights are reserved. You may not use, modify, or redistribute this code without explicit permission. Use by automated systems, including AI, is strictly prohibited.

For more details, refer to the [LICENSE](./LICENSE) file.
