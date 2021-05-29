---
layout: mypage
heading : "Configure Ansible slave - Start a service using Roles"


vcode: 556473214
---
{: .table .table-striped}
No. | Steps | Commands 
  1 | You have already cloned DevOpsMasterAnsible repository. All the code snippets for this task is placed in “10_roles” folder | git clone https://github.com/AnjuMeleth/DevOpsMasterAnsible.git
2 | Create a role in /etc/ansible/roles | sudo ansible-galaxy init demo-role
3 | Edit demo-role/tasks/main.yml files( Use file main_tasks.yml in “10_roles” folder) | sudo vi main.yml
4 | Go to handlers folder and enter the handler details in main.yml( Use file main_handlers.yml in “10_roles” folder) | sudo vi main.yml
5 | Go to files folder and create a index.html file(Use  Use file index.html file in “10_roles” folder) | sudo vi index.html
6 | Go to /etc/ansible and create a RolesDemo.yml file ( Use file RolesDemo.yml in “10_roles” folder) | sudo vi RolesDemo.yml
7 | Run the RolesDemo.yml playbook | ansible-playbook RolesDemo.yml






 
