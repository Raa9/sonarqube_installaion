# sonarqube_installaion
sonarqube installation using docker 

## install the docker 
```bash
sudo apt-get update
sudo apt-get install docker.io -y
sudo usermod -aG docker $USER   #my case is ubuntu
newgrp docker
sudo chmod 777 /var/run/docker.sock
```
## Run the sonarqube container 
```bash
docker run -d --name sonar -p 9000:9000 sonarqube:lts-community
```

## After the docker installation, we create a sonarqube container (Remember to add 9000 ports in the security group).
