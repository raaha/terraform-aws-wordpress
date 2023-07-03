# Terraform AWS WordPress

This project provides Terraform code to deploy a WordPress website on AWS infrastructure. It follows the steps outlined in the [AWS Getting Started Guide: Build a WordPress Website](https://aws.amazon.com/getting-started/hands-on/build-wordpress-website/).

## Prerequisites

Before you can use this Terraform code, make sure you have the following prerequisites:

- An AWS account
- AWS CLI installed and configured with appropriate credentials
- Terraform installed (version X.X.X)

## Deployment Steps

To deploy the WordPress website on AWS using Terraform, follow these steps:

1. Clone this repository:

```
git clone git@github.com:raaha/terraform-aws-wordpress.git
```

2. Change into the project directory:

```
cd terraform-aws-wordpress
```

3. Initialize the Terraform project:

```
terraform init
```

4. Create a `terraform.tfvars` file and customize the variables ad needed:

```
cp terraform.tfvars.example terraform.tfvars
```

Open the `terraform.tfvars` file and modify the variables to match your requirements.

5. Review the Terraform plan:

```
terraform plan
```

This step will show you the changes that Terraform will make in your AWS infrastructure.

6. Deploy the Infrastruture

```
terraform apply
```

Confirm the deployment by typing `yes` when prompted.

7. Wait for the deployment to complete. Terraform will output the website URL once the deployment is successful.

8. Access the WordPress website by visiting the URL provided.

For more details on how to build a WordPress website on AWS, refer to the [AWS Getting Started Guide: Build a WordPress Website.](https://aws.amazon.com/getting-started/hands-on/build-wordpress-website/).

## Clean Up 

To remove all the resources created by this Terraform code and destroy the infrastructure, run the follwing command:

```
terraform destroy
```