Role Name
=========

Enable either security updates or automatic updates for CentOS.

Requirements
------------

Any pre-requisites that may not be covered by Ansible itself or the role should be mentioned here. For instance, if the role uses the EC2 module, it may be a good idea to mention in this section that the boto package is required.

Role Variables
--------------
Set in the playbook:
	automatic_updates: true or security_updates: true

Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
----------------
Run with:
 ansible-playbook playbook-server-setup.yml --tags=automatic_updates -e "ansible_ssh_pass=pasword ansible_user=myusername"

Example Playbook:
- hosts: servers
  vars:
  - automatic_updates: true
  roles:
  - auto-updates

License
-------

BSD

Author Information
------------------

Meg Ford meg387@gmail.com
