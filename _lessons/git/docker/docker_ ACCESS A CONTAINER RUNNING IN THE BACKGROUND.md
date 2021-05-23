---
layout: mypage
heading : "You are working on a multi-container application and some of your containers are running in the background . But we need to access these containers for example we need to access our Ubuntu container running in the background to get to see the kernel version.How would you solve it?"

vcode: 553665110
---
{: .table .table-striped}
 No. | Steps | Commands 
 1 |Run a container in the background|sudo docker run -itd --name MyUbuntu1 ubuntu
2|Attach the container|sudo docker attach MyUbuntu1
3|List the files in the current path|ls
4|Display the kernel version|uname -srm
5|Exit the interactive terminal|exit
6|Delete the container|sudo docker rm MyUbuntu1


 
