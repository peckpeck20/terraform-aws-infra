# AWS EC2

Infrastructure as code - Terraform

## Prerequisites

- IAM credentials
- AWS CLI
- Terraform CLI

```bash

# Replace AWS_ACCESS_KEY_ID & AWS_SECRET_ACCESS_KEY with your credentials
provider "aws" {
  region = "us-west-2"
  access_key = "AWS_ACCESS_KEY_ID"
  secret_key = "AWS_SECRET_ACCESS_KEY"
}

#1
terraform init

#Format
terraform fmt

#2
terraform validate

#3
terraform plan

#4 deploy
terraform apply

#set custom variable
terraform apply -var "instance_name=customNameYO"

#Show all output values
terraform output

#Delete infrastructure
terraform destroy
```
