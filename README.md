EXPERIMENTAL - Ansible playbook to deploy Liquid Feedback
=========================================================

Requirements
------------

[Ansible](http://ansible.com) 1.9 or higher must be installed.  The easiest way
is to use Pip:

```bash
pip install ansible
```


Ansible Galaxy Roles
--------------------

This playbook depends on some open source Ansible roles from 
[Ansible Galaxy](http://galaxy.ansible.com).

```bash
ansible-galaxy -p roles/ install -r galaxy.roles
```


Run in Vagrant
--------------

First [install Vagrant from packages on the Vagrant
website](https://www.vagrantup.com/downloads.html).  Do not install Vagrant
from the Ubuntu package manager - that version is too old.

Then start Vagrant from the repo working directory:

```bash

vagrant up
```
