---
layout: mypage
heading : "You are one of the lead developers in the team. You are using an Nginx image from the Docker Hub that displays default Nginx Login page. You need to customise it with a welcome page for “DevOps Master Architect”. How would you do that?
"
vcode: 553665236
---
{: .table .table-striped}
 No. | Steps | Commands 
 1|Run a Nginx container|sudo docker run -d --name nginx1 -p 8088:80 nginx:latest
2|View the Nginx home page in browser|http://<IP address>:8088
3|Start an interactive bash terminal|sudo docker exec -it nginx1 bash
3|Modify the index page|cd /usr/share/nginx/html apt-get update apt-get install vim vim index.html
4 |Exit using Ctrl p + q | 
5 |Stop the container|sudo docker stop nginx1
6 |Start the container |sudo docker start nginx1
7 |Create a container image |sudo docker commit nginx1 YOUR_DockerHub_username/mynginx
8 |Run a container with new image that we created |sudo docker run -d --name nginx1 -p 8089:80 YOUR_username/mynginx
9|List the layers in the image|sudo docker image inspect YOUR_username/mynginx


 
