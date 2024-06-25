# terraform-project
A simple project to use Terraform to create an EC2 and Security Group

# Step-by-step Instructions on how to use Terraform

## Creating your Terraform files

1. Create the following 3 files:

- `backend.tf` - This file would be used to contain information about where to store the state file of your terraform resources.

    - Indicates what the state of the terraform resource is
    - This will usually be stored in a centralised location like S3 bucket
    - In Terraform state, the backend configuration bare minimum will need to indicate the bucket, key and region that bucket is located in

- `provider.tf` - This file would be used to contain information about which region to create your resources in.

- `main.tf` - This file would be used to contain all of the IaC to create your resources (Ec2 + Security group resources) 