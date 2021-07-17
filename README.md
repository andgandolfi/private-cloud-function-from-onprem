# Calling private Cloud Function from onprem

This repo contains a simple Terraform script to create the infrastructure described in the Medium post: <insert_link_here>

## How to run the code
* Download and Install Terraform
* Create a `terraform.tfvars` file containing the specific values for your Google Cloud environment (see `terraform.tfvars.example` file)
* Run `terraform init`
* Run `terraform apply`
* Connect to the VM in the "on-prem" project and see it can invoke the private Cloud Function (e.g. `curl https://YOUR_REGION-YOUR_PROJECT_ID.cloudfunctions.net/my-hello-function`) even if it is in a different project.
* Clean up by running `terraform destroy`