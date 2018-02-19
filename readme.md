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

Complete a Task with an added comment
-------------------------------------

`ansible-playbook complete_task.yml`

Add a Note to a Ticket in Teamwork Desk
---------------------------------------

` ansible-playbook ticket_note.yml`

To override the default variables, use --extra-vars:
----------------------------------------------------

`ansible-playbook create_project.yml --extra-vars "project_name='my new project name'"`

`ansible-playbook create_task.yml --extra-vars "task_name='my new task name'"`

`ansible-playbook complete_task.yml --extra-vars="taskId=15262488 comment='finished this task'"`

`ansible-playbook ticket_note.yml --extra-vars="ticketId=3572 body='this is a new note'"`