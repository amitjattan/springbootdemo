# springbootdemo is a MicroService applicaiton based on Springboot 1.5
Follow below isntructions to run the application and build the application docker image.

sudo apt-get install python

sudo apt-get install python-pip

sudo pip install awscli

aws configure

sudo apt-get install git

sudo git clone https://github.com/amitjattan/springbootdemo.git

sudo add-apt-repository ppa:webupd8team/java

sudo apt-get update

sudo apt-get install oracle-java8-installer

sudo apt-get install maven

cd springbootdemo

export M2_HOME=/opt/apache-maven

export PATH=${M2_HOME}/bin:${PATH}

sudo apt-get install docker.io

sudo service docker stop

sudo dockerd -H tcp://127.0.0.1:2375 &

export DOCKER_HOST=tcp://127.0.0.1:2375

sudo service docker start

mvn clean package docker:build
