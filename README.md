# **Ansible-SimpleWebApp-AWS**

## **About Ansible**

Ansible is a radically simple IT automation engine that automates cloud provisioning, configuration management, application deployment, intra-service orchestration, and many other IT needs.

## **About Project**

1.Deploying the AWS EC2 Servers as Web Servers and DB Server.

2.Installing required softwares in both servers using roles and tasks.

3.Create and configure the load balancer for the Web Servers to manage traffic

4.Finally Send the notification mail to the PIC

## **System requirements**

This version of playbooks and roles was last tested on:

Ubuntu 18.04

Python 3.8

Ansible 3.8.2

## **Infrastructure**

AWS Cloud - RHEL7

## **Development Environment**

Ubuntu WSL as Ansible Controller

## **Usage**

1.Install Ansible on Ubuntu machine

> sudo apt install ansible

2.Clone this repository

> git clone https://github.com/KevinChris7/Ansible-SimpleWebApp-AWS.git

3.Add hosts to hosts-dev inventory file

4.To Run the file

> ansible-playbook site.yml --ask-vault-pass

## **Project Insider**

- **Tasks**: A Task to deploy ec2 instances

- **Roles**: firewalldD: A role to install Firewall

- **Roles**: python: A role to install python dependencies

- **Roles**: mysqldb: A role to install and configure MySQL on any given systems

- **Roles**: flaskapp: A role to install and configure Flask application on multiple servers