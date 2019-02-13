# Install Docker

sudo apt -y install docker.io

sudo systemctl start docker

sudo systemctl enable docker

sudo usermod -aG docker ${USER}

docker --version

su - ${USER}

id -nG

docker info
