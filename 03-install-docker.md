# Install Docker

sudo apt -y install docker.io

sudo systemctl start docker

sudo systemctl enable docker

sudo usermod -aG docker ${USER}

docker --version

su - ${USER}

id -nG

docker info



# Install Docker compose

```
sudo curl -L https://github.com/docker/compose/releases/download/1.21.2/docker-compose-`uname -s`-`uname -m` -o /usr/local/bin/docker-compose

```

```
sudo chmod +x /usr/local/bin/docker-compose
```