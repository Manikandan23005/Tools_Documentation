# 📃 FreeIPA Documentation
## What is FreeIPA?
### ⚙️ FreeIPA is an open-source on-premise Identity, Policy, and Authentication (IPA) solution for Linux/Unix environments, combining LDAP, Kerberos, DNS, and certificate management to centralize authentication and access control.

## Features:

### -> LDAP-based identity directory

### -> Kerberos authentication (SSO)

### -> Host-based access control

### -> Centralized sudo rules

### -> DNS and certificate management

### -> Web UI and command-line tools

### Centralized identity and policy control
## Purpose:

###  FreeIPA provides:

### 🔹 Centralized login and user management.

### 🔹 Kerberos-based SSO for Linux clients.

### 🔹 Fine-grained access control policies.

### 🔹 On-prem solution for secure internal networks

##  Installation & Setup:

### 🔹 Install virtualization tools:
```
sudo pacman -S virt-manager qemu libvirt dnsmasq bridge-utils
sudo systemctl enable --now libvirtd
```
### 🔹 Download and install Fedora Server ISO in Virt-Manager.

### 🔹 Inside Fedora VM:
```
sudo dnf install ipa-server -y
sudo ipa-server-install --setup-dns
```
### 🔹 Follow prompts for domain, admin password, DNS, etc.

## Working:

### 🔹 FreeIPA uses Kerberos for secure authentication and LDAP for storing identity data.

### 🔹 You create users/groups and define host access policies.

### 🔹 Clients can join the FreeIPA domain to get SSO.

### 🔹 Admins manage everything via web interface or CLI.

## Conclusion:

### 🔹 FreeIPA is a powerful Linux-native IAM tool, ideal for on-premises identity management, SSO, and policy enforcement in enterprise or academic environments with multiple Linux systems.



