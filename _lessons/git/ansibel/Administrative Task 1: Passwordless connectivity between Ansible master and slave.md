---
layout: mypage
heading : Passwordless connectivity between Ansible master and slave


vcode: 556523496
---
{: .table .table-striped}
No. | Steps | Commands 
1 | Install Filezilla client Go to Edit Setting SFTP Add Keyfile Give the IP address of the master and port 22 username ubuntu Then transfer the pem file to ubuntu folder | 
2 | Stop all  firewall | sudo service ufw stop
3 | Start ssh | sudo service ssh start
4 | Add the ssh details | eval `ssh-agent -s` sudo chmod 400 yourkeyfile.pem ssh-add yourkeyfile.pem 
5 | Access the slave system from master | ssh ubuntu@IPaddress of slave node

