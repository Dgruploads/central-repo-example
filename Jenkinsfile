node 
{
  stage "1. Install docker"
  sh "sudo yum install docker -y"

  stage "2. Start the docker service"
  sh "sudo service docker start"

  stage "3. Build the docker image"
  sh "sudo docker build -t docker-image-master /home/ec2-user/"

  stage "4. Run the container"
  sh "sudo docker run -dit -p 80:80 --name docker-container-master docker-image-master"
}
