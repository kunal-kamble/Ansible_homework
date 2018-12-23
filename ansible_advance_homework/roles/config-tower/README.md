Role Name
=========

This role does the below,

       1) pre-config-tower.yml
       2) post-config-tower.yml
       3) ec2_dynamic.yml
       4) job_template.yml
       5) workflow_template.yml

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

        - name: Copy inventory vars
          copy:
            src: inventory_vars.json
            dest: /root/inventory_vars.json
        
License
-------

Opensource
