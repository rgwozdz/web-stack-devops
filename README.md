# Vagrant web-stack development-environment

## Development Environment Specs

Ubuntu 16.04  
PostgreSQL 9.5  
Nginx 1.10  
Node.js 4.2.6  
Grunt-cli 1.2.0

![image](https://raw.githubusercontent.com/rgwozdz/web-stack-devops/master/vagrant-local-dev.png?raw=true)

## Dependencies

- [Virtual Box](https://www.virtualbox.org/wiki/Downloads)

- [Vagrant](http://www.vagrantup.com/downloads)

- [Ansible](http://www.ansible.com/) >= 2.0, but see [here](https://valdhaus.co/writings/ansible-mac-osx/) for installation info.

## Creating the Vagrant VM


After installing VirtualBox and Vagrant, clone this repo:

    $ git clone https://github.com/rgwozdz/web-stack-devops.git
    
Enter the repo directory
    
    $ cd web-stack-devops

For Vagrant v1.1 or higher use:

    $ vagrant plugin install vagrant-vbguest

Now, create/boot-up the virtual machine: 
    
    $ vagrant up

By default, the initial creation of the VM with `vagrant up` with execute provisioning scripts assigned in the Vagrantfile.  To re-provision an existing VM, use `vagrant provision`.  


### Connecting to the Vagrant VM

SSH into your Vagrant VM. `cd` into web-stack-devops repo and

    $ vagrant ssh

You'll see typical Ubuntu SSH session begin.
