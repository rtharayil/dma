---
layout: mypage
heading : You are working on a high availability application deployed in a 3 node Docker Swarm cluster. For your application to handle it’s traffic you need to have at least 5 instances of Apache service up and running. How would you achieve this?

vcode: 553950161
---
{: .table .table-striped}
 No. | Steps | Commands 
 1 |Deploy an apache server |sudo docker service create --name apache2 --replicas=5 -p 8080:80 httpd
2|List the services running on the cluster |sudo docker service ls
3 |List the tasks for the service |sudo docker service ps apache2
4|List the container running on the leader node|sudo docker ps
5|Access the httpd server from any node at port 8080|
 


 
