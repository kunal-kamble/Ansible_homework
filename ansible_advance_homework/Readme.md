Role Name ❓
=========

A POC to determine the feasibility of using Ansible Tower as a CI/CD tool for 
automating continuous deployment of an internal three-tier application on QA and production environments.

Requirements 👀
===========

      1) Ansible Tower Homework Lab
      2) OpenStack for Ansible
      3) Ansible Advanced
      4) https://github.com/kunal-kamble/Ansible_homework.git


Role Variables 😎
==============

      export TOWER_GUID=e7fa
      export MYKEY=~/.ssh/mykey.pem
      export MYUSER=kunal.kamble-atos.net

Dependencies 🛒
============

  1) {{tower_guid}} is the GUID (unique identifier) i.e e7fa
  2) {{osp_guid}} is the GUID for workstation machine i.e c8bc
  3) Tower Url: [tower1.e7fa.example.opentlc.com](https://tower1.e7fa.example.opentlc.com)
  
Example Playbook 🐧
================
Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

      - hosts: localhost
        gather_facts: false 
        become: yes 
        roles:
      - config-tower

License 🔐
=======

Opensource
