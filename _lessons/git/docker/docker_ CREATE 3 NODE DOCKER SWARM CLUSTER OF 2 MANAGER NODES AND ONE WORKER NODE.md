---
layout: mypage
heading : Configure Git to include your username and email
vcode: 553949596
---
{: .table .table-striped}
 No. | Steps | Commands 
 1 |Initialise a swarm cluster|sudo docker swarm init --advertise-addr The_Ipaddress
2 |List the nodes in Docker swarm cluster |sudo docker node ls
3 |Add a worker node |git clone https://github.com/AnjuMeleth/DevOpsMasterDocker.git sh docker_install.sh sudo docker swarm join --token  _token_
4 |Go to leader node and list the nodes |sudo docker node ls
5|Get the manager token in the leader node |sudo docker swarm join-token manager
6|Add a manager node|git clone https://github.com/AnjuMeleth/DevOpsMasterDocker.git sh docker_install.sh sudo docker swarm join --token _token_


 
