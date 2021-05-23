---
layout: mypage
heading : "Your application has a CI/CD Jenkins server created as a Docker container. You created lot of jobs that runs your application pipeline.But due to some reasons your container got deleted , so all of your jobs also got deleted and could not be retrieved. How to stop such incidents happening in future?"
vcode: 553665297
---
{: .table .table-striped}
 No. | Steps | Commands 
 1|Create a volume |sudo docker volume create my-vol
2|Inspect the volume|sudo docker inspect volume my-vol
3|Run a container with a volume|sudo docker run -d --name MyJenkins -v my-vol:/var/jenkins_home -p 8090:8080 anjurose/jenkins
4|Create a freestyle job Sample|Remove the container sudo docker rm MyJenkins
6|Start a new container from same volume |sudo docker run -d --name NewJenkins -v my-vol:/var/jenkins_home -p 8091:8080 anjurose/jenkins


 
