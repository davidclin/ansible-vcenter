# /etc/ansible/vcenter.yml
This simple Ansible playbook allows you to delete VM instances from a list.
VM instances must be powered off prior to invoking this playbook. 

If the number of VM instances you need to remove is large (eg: 100+), the quick and dirty way to remove them is to get vCenter to export a list then manually copy/paste the list to this playbook. 

Steps to export list of VM's from vCenter
<pre>
(1) Highlight folder containing VM's you want to delete from disk
(2) Click the "Virtual Machines" tab
(3) Go to File -> Export -> Export List...
(4) Save as *.xls 
(5) Copy/paste VM's you want to delete to your playbook
</pre>
