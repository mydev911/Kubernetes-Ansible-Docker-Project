## install jenkins on docker on aws
#### make root user
sudo su
#### go back to user
cd
#### docker installation
yum install docker* -y
#### startt docker deamon
systemctl start docker
#### enable docker
systemctl enable docker
### now install docker 
https://www.jenkins.io/download/
#
  ```sh
  docker container ls
  docker images ls
  docker container run -itd -p 8081:8080 jenkins 
  #8081 docker port
  docker container ls
  ```
#### to find pass word for jenkins
#we need to go inside the docker container

 ```sh
 docker container exce -it (containerID) /bin/bash
 cat /var/jenkins_home/secrets/initialAdminPassword
 ```
 
  

