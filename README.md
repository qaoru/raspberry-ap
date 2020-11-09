# raspberry-ap

Ansible playbooks to setup a raspberry pi as an AP offering weak authentication
through a captive web portal, and strong authentication with 802.1X.

*At the moment, only RaspberryOS 32bits is supported.*

# Quick Start

## Declare devices

Configure your devices using `inventory.ini`.


## Install required packages and files

```
ansible-playbook -i inventory.ini -K bootstrap.yml
```

## Setup the AP

Customize your installation using `group_vars/all/all.yml`.

```
ansible-playbook -i inventory.ini -K setup.yaml
```
