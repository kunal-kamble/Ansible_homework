Role Name
=========

This roles does the below,

    1) Installs Tomcat
    2) Enables Tomcat at boot
    3) Create tomcat default web directory
    4) Copy static index.html to tomcat webroot
    5) Restart tomcat
    

Requirements
------------

1) git repository: https://github.com/kunal-kamble/Ansible_homework.git
2) Playbooks to deploy internal 3-tier app
3) Install HA Ansible Tower

Role Variables
--------------

The variables are usually inside the vars/main.yml
example: 

    payload:          tomcat
    tomcat_web_root:  /usr/share/tomcat/webapps/ROOT

Dependencies
------------

    Should be linux, Python should be installed as same version to Ansible server to avoid the modules compactibility issues
    Ansible control should be able to communicate with the host.


Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

        - name: create tomcat default web directory
          file:
            path: "{{ tomcat_web_root }}"
            state: directory

License
-------

Opensource