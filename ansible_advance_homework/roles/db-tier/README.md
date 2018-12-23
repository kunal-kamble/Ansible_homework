Role Name
=========

This role does the below,

    1) install postgres
    2) check for postgres data directories
    3) initilize postgres
    4) start postgres

Requirements
------------

  1) Ansible Tower Homework Lab
  2) OpenStack for Ansible
  3) Ansible Advanced
  4) https://github.com/kunal-kamble/Ansible_homework.git

Role Variables
--------------

     export TOWER_GUID=e7fa
     export MYKEY=~/.ssh/mykey.pem
     export MYUSER=kunal.kamble-atos.net

Dependencies
------------

    1) {{tower_guid}} is the GUID (unique identifier) i.e e8fa
    2) {{osp_guid}} is the GUID for workstation machine i.e c8bc

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - name: install postgres
      yum:
        name: postgresql-server
        state: latest

License
-------

Opensource
