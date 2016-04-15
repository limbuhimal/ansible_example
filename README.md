this is the simple example of use case of ansible.
it doesnt cover all the area of ansible like meta, vars, templates, etc but will eventually.
you can run this playbook with success with just some minor changes. 

Ansible can be seen as filesystem in unix. 

Inside the main folder (like root folder in unix filesystem): lets call this root folder in our case too, is where all the playbooks are. 

Here, I have created playbooks. if you view thesse playbooks u will see how the basic setup of 
playbook looks like.

In Playbook, YAML file:
hosts is where u indicate which servers you want your playbook to run.
roles is where u indicate which roles you want the playbook to run.

for Inventory,
I have a inventory folder, inside which i have Prod folder and inside that, I have inventory YAML file. 
You can also have inventory file at the root folder. 

Example:


----root/

	 ---->	baseSetup.yaml

	 ---->	inventory/	
                           ---->prod/
                                    ---->	inventory.yaml (this inventory file is for prod environment)

	 ---->	prodInventory(or you can directly have inventory file like this in root folder)

	 ---->	roles/

			---->commonsetup/
			---->setTime/


important terms:


	handlers: runs when called by another task.
 
	files: any files that are required by the playbook are placed in this directory   

	meta: contains dependencies

	tasks: all the task for the playbook are placed here

	vars: defines variables that are passed in tasks
              
