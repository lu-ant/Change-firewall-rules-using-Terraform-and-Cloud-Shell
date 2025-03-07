# Change-firewall-rules-using-Terraform-and-Cloud-Shell
Terraform VPC and Firewall Deployment

Overview

This repository documents the steps taken to deploy a Virtual Private Cloud (VPC) network and configure firewall rules using Terraform on Google Cloud. This lab demonstrates Infrastructure as Code (IaC) principles to ensure consistent, repeatable, and automated provisioning of cloud resources.

Scenario

Cymbal Bank is deploying a new banking application that requires a secure network environment. The team lead, Chloe, has tasked us with using Terraform to create a VPC network and configure firewall rules to control access.

Steps Completed

1. Cloning the Terraform Repository

Activated Google Cloud Shell.

Cloned the Terraform repository using the following command:

cloudshell_open --repo_url "https://github.com/terraform-google-modules/docs-examples.git" --print_file "./motd" --dir "firewall_basic" --page "editor" --tutorial "./tutorial.md" --open_in_editor "main.tf" --force_new_clone

Verified the cloned files, including main.tf.

2. Deploying the VPC and Firewall

Initialized Terraform with:

terraform init

Applied the Terraform configuration to deploy the VPC network and firewall rules:

terraform apply

Confirmed deployment by typing yes when prompted.

Verified output confirming successful deployment:

Apply complete! Resources: 3 added, 0 changed, 0 destroyed.

3. Verifying the Deployment

Navigated to VPC network > VPC networks in the Google Cloud Console.

Confirmed the test-network VPC was created.

Checked Firewalls to ensure rules were applied:

Allowed ICMP and TCP traffic on ports 80, 8080, and 1000-2000.

Key Learnings

Terraform for Cloud Automation: Automating infrastructure deployment ensures consistency and reduces manual errors.

VPC and Firewall Management: Proper firewall rules improve security and control traffic flow.

Infrastructure as Code (IaC) Best Practices: Using version-controlled configuration files helps track and manage infrastructure changes.

Conclusion

This lab provided hands-on experience in deploying a VPC network and managing firewall rules using Terraform. Automating infrastructure deployment enhances security, scalability, and efficiency in cloud environments.

✅ Successfully deployed a VPC and firewall using Terraform!
