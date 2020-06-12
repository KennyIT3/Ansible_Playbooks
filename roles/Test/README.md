Role Name
=========

This is a Test role to install packages on Redhat and Debian hosts

Requirements
------------

Redhat, Debian Host


Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

- hosts: workstation # Redhat
  become: yes
  vars:
     target_test: git
  roles:
    - Test

  handlers:
    - include_tasks: Handlers/apache.yml

#To update the Debian Host

- hosts: test_server # debian
  become: yes
  vars:
     target_test: git
  roles:
    - Test


Author Information
------------------

KennySneed
