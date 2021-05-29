---
layout: mypage
heading : You are working on a 3 node cluster with 2 manager nodes and 1 worker nodes. Due to some reason worker node was down.How would Docker handle the instances of your application running  in the worker node?
vcode: 553964354
---
{: .table .table-striped}
 No. | Steps | Commands 
 1.|List the tasks in apache 2 service in leader node |sudo docker service ps apache2
2.|Worker node leaves the swarm |sudo docker swarm leave
3.|List the tasks in apache 2 service in leader node|sudo docker service ps apache2


 
