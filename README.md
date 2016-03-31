[![Build Status](https://travis-ci.org/opsroll/ansible.svg?branch=master)](https://travis-ci.org/opsroll/ansible)

opsroll.ansible
=========

This role aims to simplify using ansible both as a developer and as an admin.

Requirements
------------

You must have already installed ansible.

Role Variables
--------------

    opsroll:
      ansible:
        user_install_path: $HOME/.ansible

Dependencies
------------



Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: localhost
      connection: local
      roles:
      - { role: opsroll.ansible, user_install_path: $HOME/.ansible }

License
-------

GPLv2

Author Information
------------------

This role was created by Charles Gardner <charles[at]opsroll.com>
