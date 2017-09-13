Test 1
-------------------------
Envrionments:
  OS: windows 10
  Docker: version 17.06.2-ce, build cec0b72 dowload from https://docs.docker.com/docker-for-windows/
  ice scrum docker img: icescrum/icescrum
  
Step 1. Install docker and enable hyper-v of windows, then restart OS
Step 2. Open powershell input below commands.
      
      # docker search icescrum/icescrum
      # docker pull icescrum/icescrum
      # docker run -d -p 80:8080 --name lmtest icescrum/icescrum 
      
      -d: Run container in background and print container ID
      Internally, iceScrum will start on port 8080. You need to map this internal port to a port of your computer in order to use iceScrum from your computer.
      As a reminder, here is how you map a port when starting a container: add -p external-port:internal-port to the docker run` command.
 
      # docker ps (Check the status of container)
      # docker stop "id"
      # docker start "id"


