Ansible Project – Deploying Docker and Containers on Multiple Hosts

This project demonstrates how to use Ansible to automate the installation and management of Docker on multiple Linux hosts with different operating systems (Ubuntu and Rocky Linux).

The playbook provisions Docker, installs required dependencies, and deploys an Nginx container using the community.docker collection.

- Features

1- Supports multiple OS families: Debian (Ubuntu) and RedHat (Rocky Linux).

2- Automates installation of Docker and dependencies.

3- Configures and enables Docker service.

4- Installs Python libraries and Docker SDK for Ansible modules.

5- Deploys an Nginx container and exposes it on port 8081.

- Tools & Technologies

1- Configuration Management: Ansible

2- Containers: Docker

3- Collection Used: community.docker

4- Target Hosts: Ubuntu (Debian family), Rocky Linux (RedHat family)

- Playbook Workflow

1-Install OS-specific dependencies

apt for Ubuntu

dnf for Rocky Linux

2-Add Docker GPG key and repository

Adds Docker’s official repo for the respective OS.

3- Install Docker packages

Installs docker-ce, docker-ce-cli, containerd.io.

4- Start and enable Docker service

Ensures Docker daemon is running and enabled at boot.

5- Install Python libraries

Installs python3, pip, and Docker SDK for Ansible integration.

6- Deploy containers

Pulls and runs an Nginx container exposed on 8081:80.


- Learning Outcomes

1- How to write OS-aware playbooks with when conditions.

2- Automating Docker installation across multiple distributions.

3- Using community.docker to manage containers directly from Ansible.

4- Deploying and testing containers as part of infrastructure automation.
