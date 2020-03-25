# Docker_Fun
##### Simple Dcoker file to crete the image and next run the container.

###### It contains two things:

- Spring boot app - fat jar (https://github.com/Wolodja/springbootwebapp)

- Dockerfile

###### There are simple steps to create and run Spring Boot app with Docker.

1) Create software folder with name "tmp"

2) Copy "spring-boot-web-0.0.1-SNAPSHOT.jar" from the target folder of the project to the tmp folder

3) In this folder copy "Dockerfile"

4) Use BASH to navigate to the folder "tmp"

5) Run "docker build -t  spring-boot-docker ."

6) After the run check if there are no errors
<br/>

#### Next run the app

- Go to docker terminal and run: docker run -d -p 8081:8081 spring-boot-docker

- Run "docker ps" if all is ok you should see:

  IMAGE                                      PORTS

  spring-boot-docker        0.0.0.0:8081->8081/tcp

###### For Windows

 - Run "docker-machine.exe ip"  and copy the IP

 - Open the browser 

 - Go to the URL bar and navigate to  "http://IP_OF_THE_CNTAINER:8081/"

Example (http://192.168.99.101:8081/) 

###### For IOS or Linux

- Use http://localhost:8081/

#### Enjoy the app!



