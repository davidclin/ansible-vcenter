# /etc/ansible/vcenter.yml
This simple Ansible playbook allows you to delete VM instances from a list.
VM instances must be powered off prior to invoking this playbook. 

If the number of VM instances you need to remove is large (eg: 100+), you can get vCenter to generate a list then manually copy/paste the list to this playbook.

