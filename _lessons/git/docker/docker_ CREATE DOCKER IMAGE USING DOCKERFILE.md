---
layout: mypage
heading : "You are working on a Python application that needs to be containerised so that it could be run everywhere without practically installing anything there. How would you achieve this?"
vcode: 553949902
---
{: .table .table-striped}
 No. | Steps | Commands 
  1 |Go to folder |cd DevOpsMasterDocker/20_CreateImage
2 |Create a Dockerfile |
3 |Build the Docker image |sudo docker build . -t anjurose/pythonapp
4|Push the image to Docker Hub |sudo docker login <br> sudo docker push anjurose/pythonapp
5 |Run a container with newly created image |sudo docker run -d --name MyApp -p 5000:5000 anjurose/pythonapp
6 |View the application running in port 5000 |http://_IpAddress_:5000





 
