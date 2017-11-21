# vcenter_vmremoval
This Ansible playbook allows you to delete VM instances from a list.
VM instances must be powered off prior to invoking this playbook. 

If number of VM instances you need to remove is large (eg: 100+), you can have vCenter generate a list for you
then manually append the list to this playbook.
