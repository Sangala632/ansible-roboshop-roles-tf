# ansible-roboshop-roles-tf

Overview
This folder contains Ansible roles and Terraform helpers used to provision and configure Roboshop infrastructure components.

Why this exists
To standardize server provisioning and role reuse across environments so services can be deployed consistently.

Workflows
- Prepare variables and inventory
- Run Terraform to provision base infra
- Run Ansible playbooks to configure services

Actions (quick start)
1. Install Terraform and Ansible.
2. Review and set variables in data.tf / vars.
3. terraform init && terraform apply
4. ansible-playbook -i inventory.ini main.yaml

Key files
- data.tf, locals.tf, main.tf, variables.tf, roles/

Notes
- Keep secrets out of repo; use Vault or encrypted vars.
