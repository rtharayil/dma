---
layout: mypage
heading : "You are working on a high availability application deployed in a 3 node Docker Swarm cluster. For your application to work efficiently you need to have an Apache server running all the nodes in a cluster. How would you achieve this?"
vcode: 553950036
---
{: .table .table-striped}
 No. | Steps | Commands 
 1 |Deploy an apache server |sudo docker service create --name apache2 --mode global -d -p 8003:80 httpd
2 |List the services running on the cluster |sudo docker service ls
3|List the tasks for the service |sudo docker service ps apache2
4|List the container running on the leader node|sudo docker ps
5|Access the httpd server from any node at port 8003| 
6|Delete the service |sudo docker service rm apache2


 
