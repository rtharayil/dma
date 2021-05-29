---
layout: mypage
heading : "You are working in an e-commerce application that is deployed in your production servers. Always the application run in “admin” user so you have to make sure you have that user in all of your production servers. How would you achieve this?
"


vcode: 556472933
---
{: .table .table-striped}
No. | Steps | Commands 
 1 |Edit /etc/hosts file in ansible master. Enter a name for slave |sudo vi /etc/hosts  Ipaddress slave1
2 |Edit /etc/ansible/hosts file | sudo vi /etc/ansible/hosts
3|Enter the details | [servers] slave1
4|Create a user in ansible slave(running the command from Ansible master)|ansible -b -m user -a 'name=admin' slave1
5|Access the ansible slave and list the users | awk -F: '{ print $1}' /etc/passwd




 
