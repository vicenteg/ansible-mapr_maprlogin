mapr_maprlogin
=========

A role that uses maprlogin to create a ticket on all nodes of a cluster.

Requirements
------------

You must have a configured, secure cluster.

Role Variables
--------------

You need to create a variable with the mapr user's clear text password. 

_Strongly_ recommended to use `ansible-vault` to encrypt the file. 

Use `--ask-vault-pass` with `ansible-playbook` to have ansible-playbook decrypt at runtime.

  mapr_user_pw_clear: my_cleartext_password

Dependencies
------------


Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: cluster
      roles:
         - { role: mapr_maprlogin, when: secure_cluster is defined and secure_cluster == True }

License
-------

MIT

Author Information
------------------

Vince Gonzalez
