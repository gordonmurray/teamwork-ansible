Teamwork Ansible
================

Some playbooks to use the Teamwork Projects API

Examples
--------

First, update teamwork_projects_url and teamwork_projects_api_key in /roles/vars/main.yml.

Create a new Project
--------------------

`ansible-playbook create_project.yml`

Create a Task in a Tasklist
---------------------------

`ansible-playbook create_task.yml`

To override the default variables, use --extra-vars:

`ansible-playbook create_project.yml --extra-vars "project_name='my new project name'"`