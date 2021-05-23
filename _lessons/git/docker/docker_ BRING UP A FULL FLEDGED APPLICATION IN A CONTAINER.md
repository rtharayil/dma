---
layout: mypage
heading : "You are the lead developer of your team and you are requested to set up a CI/CD server (JENKINS) for your application fastly. How would you solve it?"
vcode: 553665141
---
{: .table .table-striped}
 No. | Steps | Commands 
 1 |Run the Jenkins container |sudo docker run --name jenkins -p 8085:8080 anjurose/jenkins
2|View the Jenkins dashboard in the browser |Access your application at  YOUR_ipaddress:8085
3 |Stop the container and exit it by Ctrl + c command | Ctrl + c
4 |View the containers |sudo docker ps -a


 
