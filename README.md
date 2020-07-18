# EDX
we need to understand , we need to install some tools<br/>
first thing we need to know is to install python, setup<br/>
docker and git the link. somehow edx is a web based on python<br/>
the second thing we need to know is the environment, the environment was docker<br/>
i using python3 for deploy edx site, curl windows.<br/>

#step to configure 
because this site is the python based website, its must install python first<br/>
python web usualy use django, django its like apache django is a service to take care<br/>
the web.so here it is the syntax.
# install python
``` sudo apt install python3
sudo apt install python3-pip
sudo cp /usr/bin/pip3 /usr/bin/pip
```

# to install make
sudo apt install make

# install docker
```sudo apt install apt-transport-https ca-certificates curl software-properties-common
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu bionic stable"
sudo apt update
apt-cache policy docker-ce
sudo apt install docker-ce
sudo apt install docker-compose
```

# syntax for run docker without using sudo
```sudo usermod -aG docker ${USER}
su - ${USER}
id -nG
```

# install git + clone
```sudo apt install git
git clone https://github.com/edx/devstack
```

# to run every service
```cd devstack
make requirements
make dev.provision
make dev.up
```
