---
layout: mypage
heading : "You are working in an e-commerce application that is deployed in your production servers. Always the application run in “admin” user so you have to make sure you have that user in all of your production servers. How would you achieve this?
"


vcode: 556528698
---
{: .table .table-striped}
No. | Steps | Commands 
  1 | Install an Nginx package on slave | ansible -b -m package -a 'name=nginx state=present' slave1
2 | Start Nginx service on slave | ansible -b -m service -a 'name=nginx state=started' slave1
3 | View the Nginx service on slave | Give the Ip address of slave in the browser
4 | Stop the service in slave | ansible -b -m service -a 'name=nginx state=stopped' slave1





 
