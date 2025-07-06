# CyberArk Conjur Documentation

## What is CyberArk Conjur?
### CyberArk Conjur is a free and open-source secrets management solution by CyberArk, designed for DevOps and CI/CD pipelines. It secures credentials, API keys, and database passwords used by applications and containers.

## Features:

### -> Secrets management with strict RBAC

### -> Secure storage of passwords, API keys, certificates

### -> REST API and CLI for integration

### -> Policy-based access control

### -> Works with Docker, Kubernetes, Jenkins, Ansible, etc.

### -> Open source and scalable

## Purpose:

###  Conjur protects:

### 🔹 Secrets used in automation pipelines

### 🔹 Infrastructure credentials in containers

### 🔹 Access keys in cloud-native apps

###  Installation & Setup:

### 🔹 Install Docker:
```
sudo pacman -S docker docker-compose
sudo systemctl start docker
sudo systemctl enable docker
```
### 🔹 Clone Conjur Quickstart:
```
git clone https://github.com/cyberark/conjur-quickstart
cd conjur-quickstart
./start.sh
```
### 🔹 Load policies and test secrets:
```
./load_policy.sh
conjur variable values add db/password MySuperSecret123
```
### 🔹 Retrieve secrets with:
```
conjur variable value db/password
```
## Working:

### 🔹 Secrets are stored in the encrypted Conjur Vault.

### 🔹 Access to secrets is controlled by policy files.

### 🔹 Apps or users authenticate via tokens and retrieve secrets via REST API.

### 🔹 All access is logged and auditable

## Conclusion:

### 🔹 CyberArk Conjur is ideal for DevOps teams who need a lightweight, programmable, and secure way to manage secrets in pipelines, containers, and automation tools.


