# /etc/ansible/vcenter.yml
This simple Ansible playbook allows you to spin up a VM using a template.

This playbook also allows you to delete VM instances from a list.

To delete VM instances from a list, the VM instances must be powered off prior to invoking this playbook. 

If the number of VM instances you need to remove is large (eg: 100+), the quick and dirty way to remove them is to export a list from vCenter then manually copy/paste the VM list to this playbook. 

Steps to export list of VM's from vCenter
<pre>
(1) Highlight folder containing VM's you want to delete from disk
(2) Click the "Virtual Machines" tab
(3) Go to File -> Export -> Export List...
(4) Save as *.xls 
(5) Copy/paste VM's you want to delete to your playbook
</pre>

Useful Commands
<pre>
ansible-playbook vcenter.yml 
ansible-playbook vcenter.yml --tags "deploy_vm"
ansible-playbook vcenter.yml --tags "delete_vms"
</pre>
