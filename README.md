[![Build Status](https://travis-ci.org/opsroll/ansible.svg?branch=master)](https://travis-ci.org/opsroll/ansible)

opsroll.ansible
=========

This role aims to simplify using ansible both as a developer and as an admin.

Requirements
------------

- Ansible installed via PIP
- A basic configuration at ~/.ansible.cfg

    [defaults]
    roles_path=$HOME/.ansible/roles/galaxy
    hash_behaviour = merge


Role Variables
--------------

    opsroll:
      ansible:
        user_install_path: $HOME/.ansible

Dependencies
------------



Example Setup Playbook
----------------------

The quick setup goes as follows. Create a file in your $HOME directory called
.setup.yml and paste the following into it.

      - hosts: localhost
        connection: local
        roles:
        - { role: opsroll.ansible, user_install_path: $HOME/.ansible }

then run it

      `ansible-playbook ~/.setup.yml`

now your ansible is configured to run completely within your home directory.

License
-------

GPLv2

Author Information
------------------

This role was created by Charles Gardner <charles[at]opsroll.com>
