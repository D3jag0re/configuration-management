# configuration-management

This is based off the DevOps Roadmap Project [Configuration Management](https://roadmap.sh/projects/configuration-management)

Write an Ansible playbook to configure a Linux server. 

This is number 12 of [DevOps Projects](https://roadmap.sh/devops/projects) as per roadmap.sh

## Description From Site 

The goal of this project is to introduce you to the basics of configuration management using Ansible. You will write an Ansible playbook to configure a Linux server.

## Requirements

If you have been doing the previous projects, you should already have a Linux server running. If not, setup a Linux server on DigitalOcean, AWS or another cloud provider.

You are required to write an Ansible playbook called setup.yml and create the following roles:

- `base` — basic server setup (installs utilities, updates the server, installs fail2ban, etc.)
- `nginx` — installs and configures nginx
- `app` — uploads the given tarball of a static HTML website to the server and unzips it.
- `ssh` - adds the given public key to the server

Set up the inventory file inventory.ini to include the server you are going to configure When you run the playbook, it should run the roles above in sequence. You should also assign proper tags to the roles so that you can run only specific roles.

## To Run 

- Setup the following repository secrets:
    - DO_TOKEN : Digital Ocean access token
    - DO_SPACES_SECRET_KEY : Digital Ocean spaces secret key (for Terraform state file)
    - DO_SPACES_ACCESS_KEY : Digital Ocean spaces access key (for Terraform state file)
    - DO_SSH_PUBLIC_KEY : Keypair to be used for VM 
    - DO_SSH_PRIVATE_KEY : Keypair to be used for VM

- Run workflow: This will build and install everything.
- Access webpage from `http://<ip_address>` 


## Notes 

- Going to use terraform to build droplet 

## Lessons Learned

- Lesson.
