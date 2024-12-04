# Server Setup
~ TODO: Include mdatp tasks 

## Project Overview

This project is designed for the initial configuration of a new server, with the expectation of a single execution to establish the full setup. However, it has been structured modularly, so specific roles can be executed independently if necessary. This modular design facilitates the reset of any server component to its original post-installation state.

## Requirements
+ `python3`
+ `ansible>=2.9`
> See INSTALL.md for instructions on installing Ansible

## Getting Started

To run this project:

1. Ensure Ansible is installed on your control node.
2. Configure the  `inventory.ini` file with the server details.
3. Run the playbook with the following command:

    ```shell
    ansible-playbook -i ansible-playbook main.yml
    ```

## Project Structure

The project is divided into roles, each responsible for a different aspect of server configuration:

+ **access-control**: Configures SSH and sudo policies.
+ **accessibility**: Sets hostname, keyboard layout, locale, NTP, and timezone.
+ **active-directory**: Adds relevant DNS records(A and PTR), creates AD groups and takes care of joining the server to the domain.
+ **mail**: Installs and configures postfix for mail alerts.
+ **monitoring**: Auditing configuration and policies are defined here.
+ ~~**network**: Configures netplan to use a static IP.~~
+ **security**: Configures various security tools.
+ **user-management**: Account creation and user policies defined here.
