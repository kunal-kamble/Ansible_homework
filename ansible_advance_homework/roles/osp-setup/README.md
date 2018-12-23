Role Name
=========

This role does the following below,

        1) create-image.yml
        2) create-flavor.yml
        3) create-keypair.yml
        4) create-network.yml
        5) create-sg.yml

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

        1) {{tower_guid}} is the GUID (unique identifier) i.e e7fa
        2) {{osp_guid}} is the GUID for workstation machine i.e c8bc

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

        - name: Download RHEL image
          get_url:
             url: http://www.opentlc.com/download/osp_advanced_networking/rhel-guest-image-7.2-20151102.0.x86_64.qcow2
             dest: /tmp/rhel.qcow2
          tags:
              - tested
License
-------

Opensource
