---
layout: mypage
heading : You have created a Docker image that needs to stored for future uses. How would you solve it?

vcode: 553665431
---
{: .table .table-striped}
 No. | Steps | Commands 
 1 |Login to the DockerHub |sudo docker login
2|Push the image to DockerHub|sudo docker push YOUR_username/mynginx
3 |Delete the image from your machine|sudo docker rmi YOUR_username/mynginx
4|If a running image is using the image we cannot delete the image so stop the container running and remove the image |sudo docker rm -f nginx1 sudo docker rmi YOUR_username/mynginx


 
