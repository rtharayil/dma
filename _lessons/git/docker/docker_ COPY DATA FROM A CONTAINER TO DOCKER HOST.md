---
layout: mypage
heading : "Being a DevOps practitioner, you brought up a Jenkins container but forgot to add volumes. How can you safely copy the data in your container to your Docker Host?"
vcode: 553949436
---
{: .table .table-striped}
 No. | Steps | Commands 
 1 |Create a directory in host system |mkdir copied_data
2 | Run the Jenkins Container and create a job |sudo docker run --name MyJenkins2 -p 8080:8080 anjurose/jenkins
3 |Copy the files |sudo docker cp MyJenkins2:/var/jenkins_home ./copied_data
4|Remove the container|sudo docker rm -f MyJenkins2


 
