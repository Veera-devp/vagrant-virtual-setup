# Vagrant Virtual Setup

## Overview

This repository contains Vagrant configuration files for setting up development environments. It provides two configurations:

### CentOS Stream 9

#### Description

This Vagrant configuration sets up a CentOS Stream 9 environment with the following features:

- Forwarded port mapping for accessing port 80 on the guest machine via `localhost:8080`.
- Private network with the IP address `192.168.33.11`.
- Public network for bridged networking.
- Additional provisioning using a shell script to install `httpd`, `wget`, `unzip`, `vim`, and deploy a template.

#### Usage

1. Ensure you have Vagrant and VirtualBox installed.
2. Clone this repository.
3. Navigate to the directory containing the Vagrantfile.
4. Run `vagrant up` to start the VM.

### WordPress on Ubuntu

#### Description

This Vagrant configuration sets up an Ubuntu environment with WordPress installed. It includes the following features:

- Forwarded port mapping for accessing port 80 on the guest machine via `localhost:8080`.
- Private network with the IP address `192.168.33.10`.
- Public network for bridged networking.
- Additional provisioning using a shell script to install and configure Apache, MySQL, PHP, and WordPress.

#### Usage

1. Ensure you have Vagrant and VirtualBox installed.
2. Clone this repository.
3. Navigate to the directory containing the Vagrantfile.
4. Run `vagrant up` to start the VM.

#### Accessing WordPress

After provisioning, WordPress can be accessed at [http://192.168.33.10/wordpress](http://192.168.33.10/wordpress).

- Database name: wordpress
- Database username: wordpress
- Database password: raghava

#### Notes

This setup is intended for development purposes only and is not suitable for production environments.
