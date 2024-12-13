# Homelab
This is set up to be a simple demonstration of how I have my home lab configured for home security, malware analysis and personal technical growth.

Inside, we deploy a secure enviornment with industry-leading technologies including Terraform, Ansible, Proxmox; giving us the ability to control an easily collapseable and highly scaleable security sandbox. This is a short list of technologies we will be using in our homelab. 



## Proxmox (The Hypervisor)
This is an excellent opensource hypervisor, but I probably don't need to tell you that. We will using proxmox for its pricing (free for life) and its API support

https://www.proxmox.com/en/


## Docker
- A common container service that we will use to host various servers
- Great for easliy spinning up and destorying web apps for penetration testing purposes

https://www.docker.com/


## Jumpbox
Our jump box will act as our jumping off point when we interactive wiht our sandbox. We will be using KDE neon for its ease of use and wide range of Debian based tools and repositories

https://neon.kde.org/


## Jumpbox Tooling
VS Code
- This is essintial when working with devops tools
- Ansible extension
- HashiCorp Terraform extension
- HashiCorp HCL extension

https://code.visualstudio.com/


## HashiCorp Tools
- Packer to create VM templates
- Terraform uses Packer templates to deploy one or more virtual machines
- Vault for keeping our secrets

https://www.hashicorp.com/


## Ansible
- Ansible configures our devices after Terraform deploys them
- This is how we will set up our playbooks for a consistant deployment

sudo apt install -y python3-pip sshpass && pip3 install ansible hvac


## Remote Desktop
- We will be using KRDC as it is the natie KDE remote desktop tool
sudo apt install -y krdc


# Operating Systems

## Kali Linux
This will be the attack box that we use for various projects

https://www.kali.org/
