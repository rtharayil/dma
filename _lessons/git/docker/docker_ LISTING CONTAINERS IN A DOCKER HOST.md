---
layout: mypage
heading : "You are working on an application that uses microservices architecture. So you have a lot of containers working at a time. How would you list all running containers and stopped containers."
vcode: 553665385
---
{: .table .table-striped}
 No. | Steps | Commands 
 1 |Run a container |sudo docker run --name MyUbuntu ubuntu
2|List all the containers in the Docker host|sudo docker ps -a
3|Run a container with an open interactive terminal |sudo docker run -it --name MyUbuntu1 ubuntu
4|Come out of the terminal without stopping the container by Ctrl P + Q| 
5|Run a container with an open interactive terminal |In the background sudo docker run -it --name MyUbuntu2 ubuntu
6|List all the running containers in the Docker host|sudo docker ps -a


 
