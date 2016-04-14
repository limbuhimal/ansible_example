this is the simple example of use case of ansible.
it doesnt cover all the area of ansible like meta, vars, templates, etc.
Although, if you run this playbook with correct inventory, it will run with success. 

Ansible can be seen as filesystem in unix. 

Inside the main folder (like root folder in unix) is where all the playbooks are. 
here, basesetup.yaml is my playbook. if you view this playbook u will see what the basic setup of 
playbook looks like.

In Playbook, YAML file:
hosts is where u indicate which servers you want your playbook to run.
roles is where u indicate which roles you want the playbook to run.

