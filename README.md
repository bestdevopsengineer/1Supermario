# Supermario
terraform + [sonarqube+EC2]+ Dockerhub + aquatrivy + [AKS+ArgoCD]

provider "azurerm" {
  features {}
  subscription_id = "<your_subscription_id>"
  client_id       = "<your_client_id>"
  client_secret   = "<your_client_secret>"
  tenant_id       = "<your_tenant_id>"
}

or

export ARM_SUBSCRIPTION_ID=<your_subscription_id>
export ARM_CLIENT_ID=<your_client_id>
export ARM_CLIENT_SECRET=<your_client_secret>
export ARM_TENANT_ID=<your_tenant_id>

az login --tenant TENANT_ID
GOTO home/default directory/app registration

terraform init
terraform plan -var-file="vars/east-us-2.tfvars"
terraform apply -var-file="vars/east-us-2.tfvars" --auto-approve