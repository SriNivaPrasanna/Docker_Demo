"# Docker_Demo"

1.We Can create EC2 instance for Ubuntu AMI
2.Open a GIT & select sshid
3.Remove any Docker files that are running in the system, using the following command: 
$ sudo apt-get remove docker docker-engine docker.io 
After entering the above command, you will need to enter the password of the root and press enter. 
4.Check if the system is up-to-date using the following command: 
$ sudo apt-get update 
5 Install Docker using the following command: 
$ sudo apt install docker.io 
You’ll then get a prompt asking you to choose between y/n - choose y 
Learn Concepts - Basics to Advanced! 
Caltech Program in DevOpsEXPLORE PROGRAMLearn Concepts - Basics to Advanced! 
6 Install all the dependency packages using the following command: 
$ sudo snap install docker 
7 Before testing Docker, check the version installed using the following command: 
$ Sudo docker --version
6.Pull an image from the Docker hub using the following command: 
$ sudo docker run hello-world 
Here, hello-world is the docker image present on the Docker hub.
7.Check if the docker image has been pulled and is present in your system using the following command:
 $ sudo docker images
8.To display all the containers pulled, use the following command: 
$ sudo docker ps -a
9.To check for containers in a running state, use the following command: 
$ sudo docker ps 
You’ve just successfully installed Docker on Ubuntu! 
Create docker file & Run Docker images & Docker Container 
10.Create directory myapp
11.create demo.html file "Hello-World"
12.create Dockerfile content below 
FROM nginx 
COPY demo.html /usr/share/nginx/html
13.Build a Docker file in a Docker image 
$ sudo docker build -t myapp . 
14.Run a Docker file in a Docker image 
$ sudo docker run -d -p 8080:80 myapp . 
15.Run a Docker file in Web browser http://localhosts:8080 do WebBrowser 
