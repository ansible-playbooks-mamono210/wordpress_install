[![](https://github.com/ansible-playbooks-centos7/wordpress_install/workflows/ansible-lint/badge.svg)](https://github.com/ansible-playbooks-centos7/wordpress_install/actions?query=workflow%3Aansible-lint)
[![](https://github.com/ansible-playbooks-centos7/wordpress_install/workflows/trailing%20whitespace/badge.svg)](https://github.com/ansible-playbooks-centos7/wordpress_install/actions?query=workflow%3A%22trailing+whitespace%22)
[![](https://github.com/ansible-playbooks-centos7/wordpress_install/workflows/molecule/badge.svg)](https://github.com/ansible-playbooks-centos7/wordpress_install/actions?query=workflow%3Amolecule)
[![](https://github.com/ansible-playbooks-centos7/wordpress_install/workflows/yamllint/badge.svg)](https://github.com/ansible-playbooks-centos7/wordpress_install/actions?query=workflow%3Ayamllint)

# Ansible Playbook - Wordpress Install

## Introduction

This program installs [WordPress](https://wordpress.com) on CentOS7.

## How To install

1. Install ansible and git

```
sudo yum -y install epel-release git
sudo yum -y install ansible
```

2. Execute playbook as root

```
git clone https://github.com/ansible-playbooks-centos7/wordpress_install.git
cd wordpress_install
ansible-galaxy install -r roles/requirements.yml
ansible-playbook -i localhost, -c local install.yml
```
