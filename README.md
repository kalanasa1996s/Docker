# Docker 


AWS - Run Docker in EC2
  
  1).Create AWS Instance (ubuntu)
  
      https://aws.amazon.com/
  
  2).Insatll Docker
  
      https://docs.docker.com/engine/install/ubuntu/
 
 ---------------------------------------------------------------------------------------
  3).Check Docker Images
      
      docker images
  
  4).check running docker container
  
      docker ps
      
  5).check all docker container
  
      docker ps -a ( get access - chmod 666 /var/run/docker.sock)
      
 ---------------------------------------------------------------------------------------
 
 Local Project Send to Server -------
 
  1).scp -r -i yourawskey.pem dockerprojectdirectory instancename@......com:~/ ( "/" -> root )
  
    Upload your docker project to server
  
  2).Build Docker Image 
  
    docker build -t myfirstimg .  (go in your docker folder)
 
  3).check docker image
  
      docker images
      
 4).create & run docker container
 
      docker run myfirstimg
      --------------------------
      exit (exit docker container)
      
 5). run this container
  
    docker ps -a  (show all docker containers)
    
    docker start -i containerid
    
---------------------------------------------------------------------------------------

7).delete docker image

    docker image rmi -f imageName
    
8).delete containers
    
    docker rm containerid
    
    
    

      
