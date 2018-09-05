# springbootdemo is a MicroService application based on Springboot 1.5
Follow below set of commands to build the application image from docker.

sudo apt-get install python-pip python-dev build-essential 

sudo pip install --upgrade pip 

sudo pip install --upgrade virtualenv 

sudo pip install awscli

aws configure

sudo apt-get install git

sudo add-apt-repository ppa:webupd8team/java

sudo apt-get update

sudo apt-get install oracle-java8-installer

sudo apt-get install maven

export M2_HOME=/usr/share/maven

export PATH=${M2_HOME}/bin:${PATH}

sudo apt-get install docker.io

sudo service docker stop

#dockerd -H tcp://127.0.0.1:2375 &

export DOCKER_HOST=unix:///var/run/docker.sock

#export DOCKER_HOST=tcp://127.0.0.1:2375

sudo service docker start

docker images

sudo git clone https://github.com/amitjattan/springbootdemo.git

cd springbootdemo

mvn clean package docker:build
