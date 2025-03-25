# Webmin
Ansible playbook installs Webmin on Redhat, Rocky9 and Ubuntu and configures Webmin to listen on port 59153, port number can be changed to any other port requirements in the playbook setup-webmin.yml.

## Overview
Webmin is a web-based interface for system administration for Unix. Using any modern web browser, you can set up user accounts, Apache, DNS, file sharing, and much more. Webmin removes the need to manually edit Unix configuration files like `/etc/passwd`, and lets you manage a system from the console or remotely.

## Features
- **User Management:** Easily create, modify, and delete user accounts.
- **File Management:** Access and manage the file system, upload and download files, and edit text files.
- **Service Control:** Start, stop, and restart services like Apache, MySQL, and others.
- **System Monitoring:** Monitor system resources like CPU, memory, and disk usage.
- **Package Management:** Install, update, and remove packages using your system’s package manager.
- **Network Configuration:** Configure network interfaces, firewall rules, and more.
- **Security:** Manage users, groups, permissions, and security policies.

## Requirements
- A Unix-like operating system (Linux, BSD, Solaris, etc.)
- A modern web browser (Chrome, Firefox, Edge, etc.)

## Prerequisite

Edit the inventory file for you hosts, unless running the playbook local.

Install
[Ansible Community General Collection](https://github.com/ansible-collections/community.general)
ansible-galaxy collection install community.general 

### Using the Ansible Playbook Installation
The easiest way to install Webmin is to clone the repo and run the playbook:

```
git clone git@github.com:allenjoey/ansible-webmin.git
ansible '*' -m ping (Pint Test)
ansible-playbook setup-webmin.yml -v

```
## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License
[MIT](https://choosealicense.com/licenses/mit/)

## Author Information

Joey Allen